---
title: Instalar o Microsoft Graph PowerShell SDK
description: Fornece instruções para instalar o Microsoft Graph PowerShell SDK.
ms.localizationpriority: medium
author: jasonjoh
ms.openlocfilehash: 80086e4879ce9acb547e060c45891bd58dc602bf
ms.sourcegitcommit: 0fa7148e0b776663eaca3e79e72b85046d4b8b1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/15/2022
ms.locfileid: "63500956"
---
# <a name="install-the-microsoft-graph-powershell-sdk"></a>Instalar o Microsoft Graph PowerShell SDK

> [!NOTE]
> A instalação do módulo principal do SDK instalará todos os 38 sub módulos. Considere apenas instalar os módulos necessários, incluindo `Microsoft.Graph.Authentication`. Para uma lista de módulos Graph Microsoft disponíveis, use o comando a seguir.
>
> ```powershell
> Find-Module Microsoft.Graph*
> ```

O Microsoft Graph SDK do PowerShell é publicado na [Galeria do PowerShell](https://www.powershellgallery.com/packages/Microsoft.Graph). Você pode instalar o SDK no PowerShell Core ou Windows PowerShell usando o comando a seguir.

```powershell
Install-Module Microsoft.Graph -Scope CurrentUser
```

Opcionalmente, você pode alterar o escopo da instalação usando o `-Scope` parâmetro. Isso requer permissões de administrador.

```powershell
Install-Module Microsoft.Graph -Scope AllUsers
```

> [!IMPORTANT]
> Instalar o SDK em uma versão do PowerShell não o instala para a outra. Certifique-se de executar o comando de instalação dentro da versão do PowerShell em que você pretende usá-lo.

## <a name="supported-powershell-versions"></a>Versões com suporte do PowerShell

O PowerShell 7 e posterior é a versão recomendada do PowerShell para uso com o Microsoft Graph SDK do PowerShell em todas as plataformas. Não há pré-requisitos adicionais para usar o SDK com o PowerShell 7 ou posterior.

Os seguintes pré-requisitos devem ser atendidos para usar o Microsoft Graph SDK do PowerShell com Windows PowerShell.

- Atualizar para [o PowerShell 5.1 ou posterior](/powershell/scripting/windows-powershell/install/installing-windows-powershell#upgrading-existing-windows-powershell)
- Instalar [.NET Framework 4.7.2 ou posterior](/dotnet/framework/install/)
- Atualizar **o PowerShellGet** para a versão mais recente usando `Install-Module PowerShellGet -Force`

## <a name="verify-installation"></a>Verificar a instalação

Após a conclusão da instalação, você pode verificar a versão instalada com o comando a seguir.

```powershell
Get-InstalledModule Microsoft.Graph
```

A versão na saída deve corresponder à versão mais recente publicada na Galeria do PowerShell. Agora você está pronto para usar o SDK.

> [!div class="nextstepaction"]
> [Comece a usar o SDK do Microsoft Graph PowerShell](get-started.md)

## <a name="updating-the-sdk"></a>Atualizando o SDK

Você pode atualizar o SDK e todas as suas dependências usando o comando a seguir.

```powershell
Update-Module Microsoft.Graph
```

## <a name="uninstalling-the-sdk"></a>Desinstalar o SDK

Primeiro, use o seguinte comando para desinstalar o módulo principal.

```powershell
Uninstall-Module Microsoft.Graph
```

Em seguida, remova todos os módulos de dependência executando os seguintes comandos.

```powershell
Get-InstalledModule Microsoft.Graph.* | %{ if($_.Name -ne "Microsoft.Graph.Authentication"){ Uninstall-Module $_.Name } }
Uninstall-Module Microsoft.Graph.Authentication
```

## <a name="provide-feedback"></a>Faça comentários

Comentários de boas-vindas! Forneça comentários ou informe quaisquer problemas no [repositório de GitHub SDK](https://github.com/microsoftgraph/msgraph-sdk-powershell/issues).
