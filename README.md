-- Script para conceder acesso premium no jogo CARROSEL

-- Função para conceder acesso premium ao jogador
local function concederAcessoPremium(jogador)
    -- Conceder acesso a todos os recursos premium
    print(jogador.Name .. " tem acesso premium!")
    -- Adicione aqui os recursos premium que você deseja conceder
    -- Exemplo: jogador:GiveTool(game.ServerStorage.PremiumTool)
end

-- Conectar a função ao evento de jogador adicionado
game.Players.PlayerAdded:Connect(function(jogador)
    -- Simular que o jogador tem assinatura premium
    jogador.MembershipType = Enum.MembershipType.Premium
    concederAcessoPremium(jogador)
end)
