---
title: Instalar o SDK do Microsoft Graph PowerShell
description: Fornece instruções para instalar o SDK do Microsoft Graph PowerShell.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 245cf03c8edf04a43c563bd19832eb0a35cf7cff
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193645"
---
# <a name="install-the-microsoft-graph-powershell-sdk"></a>Instalar o SDK do Microsoft Graph PowerShell

O SDK do Microsoft Graph PowerShell é publicado na [Galeria do PowerShell](https://www.powershellgallery.com/packages/Microsoft.Graph). Você pode instalar o SDK no PowerShell core ou no Windows PowerShell usando o seguinte comando.

```powershell
Install-Module Microsoft.Graph
```

Opcionalmente, você pode alterar o escopo padrão da instalação usando o `-Scope` parâmetro. Isso exige permissões de administrador.

```powershell
Install-Module Microsoft.Graph -Scope AllUsers
```

> [!IMPORTANT]
> A instalação do SDK em uma versão do PowerShell não o instala para o outro. Certifique-se de executar o comando de instalação dentro da versão do PowerShell em que você pretende usá-lo.

## <a name="verify-installation"></a>Verificar a instalação

Após a conclusão da instalação, você pode verificar a versão instalada com o seguinte comando.

```powershell
Get-InstalledModule Microsoft.Graph
```

A versão na saída deve corresponder à versão mais recente publicada na galeria do PowerShell. Agora você está pronto para usar o SDK.

> [!div class="nextstepaction"]
> [Introdução ao SDK do Microsoft Graph PowerShell](get-started.md)

## <a name="updating-the-sdk"></a>Atualizando o SDK

Você pode atualizar o SDK e todas as suas dependências usando o comando a seguir.

```powershell
Update-Module Microsoft.Graph
```

## <a name="uninstalling-the-sdk"></a>Desinstalando o SDK

Primeiro, use o comando a seguir para desinstalar o módulo principal.

```powershell
Uninstall-Module Microsoft.Graph
```

Em seguida, remova todos os módulos de dependência executando os seguintes comandos.

```powershell
Get-InstalledModule Microsoft.Graph.* | %{ if($_.Name -ne "Microsoft.Graph.Authentication"){ Uninstall-Module $_.Name } }
Uninstall-Module Microsoft.Graph.Authentication
```

## <a name="provide-feedback"></a>Faça comentários

Agradecemos comentários! Forneça comentários ou Informe qualquer problema no [repositório do GitHub do SDK](https://github.com/microsoftgraph/msgraph-sdk-powershell/issues).
