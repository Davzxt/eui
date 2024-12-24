local textureId = "6403436082"

function replaceTextures()
    for _, part in pairs(game.Workspace:GetDescendants()) do
        if part:IsA("BasePart") then
            local surfaceGui = Instance.new("SurfaceGui", part)
            surfaceGui.Face = Enum.NormalId.Front
            local imageLabel = Instance.new("ImageLabel", surfaceGui)
            imageLabel.Size = UDim2.new(1, 0, 1, 0)
            imageLabel.Image = textureId
        end
    end
end

replaceTextures()
