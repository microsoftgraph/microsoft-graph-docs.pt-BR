---
title: Instalar o Microsoft Graph PowerShell SDK
description: Fornece instruções para instalar o Microsoft Graph PowerShell SDK.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 58e967d7acedbbfe4f8c3781a7ec796e697a44c8
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107673"
---
# <a name="install-the-microsoft-graph-powershell-sdk"></a>Instalar o Microsoft Graph PowerShell SDK

> [!NOTE]
> A instalação do módulo principal do SDK instalará todos os 38 sub módulos. Considere apenas instalar os módulos necessários, incluindo `Microsoft.Graph.Authentication` .

O SDK do Microsoft Graph PowerShell é publicado na [Galeria do PowerShell.](https://www.powershellgallery.com/packages/Microsoft.Graph) Você pode instalar o SDK no PowerShell Core ou Windows PowerShell usando o comando a seguir.

```powershell
Install-Module Microsoft.Graph -Scope CurrentUser
```

Opcionalmente, você pode alterar o escopo da instalação usando o `-Scope` parâmetro. Isso requer permissões de administrador.

```powershell
Install-Module Microsoft.Graph -Scope AllUsers
```

> [!IMPORTANT]
> Instalar o SDK em uma versão do PowerShell não o instala para a outra. Certifique-se de executar o comando de instalação dentro da versão do PowerShell em que você pretende usá-lo.

## <a name="verify-installation"></a>Verificar a instalação

Após a conclusão da instalação, você pode verificar a versão instalada com o comando a seguir.

```powershell
Get-InstalledModule Microsoft.Graph
```

A versão na saída deve corresponder à versão mais recente publicada na Galeria do PowerShell. Agora você está pronto para usar o SDK.

> [!div class="nextstepaction"]
> [Começar com o Microsoft Graph PowerShell SDK](get-started.md)

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

Comentários de boas-vindas! Forneça comentários ou informe quaisquer problemas no [repositório GitHub SDK.](https://github.com/microsoftgraph/msgraph-sdk-powershell/issues)
