---
title: Criar windowsAssignedAccessProfile
description: Crie um novo objeto de windowsAssignedAccessProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2313dff2c2f387e0a981775e0b6cc6e53a988f3f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956343"
---
# <a name="create-windowsassignedaccessprofile"></a>Criar windowsAssignedAccessProfile

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Crie um novo objeto de [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) .
## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto windowsAssignedAccessProfile.

A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsAssignedAccessProfile.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|profileName|Cadeia de caracteres|Este é um nome amigável usado para identificar um grupo de aplicativos, o layout desses aplicativos no menu Iniciar e os usuários aos quais essa configuração de quiosque é atribuída.|
|showTaskBar|Booliano|Essa configuração permite que o administrador especificar se a barra de tarefas é mostrada ou não.|
|appUserModelIds|String collection|Estes são os únicos repositório aplicativos do Windows que estarão disponíveis para início no menu Iniciar.|
|desktopAppPaths|String collection|Estes são os caminhos dos aplicativos de área de trabalho que estarão disponíveis no menu Iniciar e os aplicativos somente o usuário será capaz de início.|
|userAccounts|String collection|As contas de usuário que serão bloqueadas para esta configuração de quiosque.|
|startMenuLayoutXml|Binária|Permite que os administradores substituir o layout de início padrão e impede que o usuário alterá-la.O layout é modificado especificando um arquivo XML com base em um esquema de modificação de layout. XML deve estar em formato binário.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles
Content-type: application/json
Content-length: 364

{
  "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
  "profileName": "Profile Name value",
  "showTaskBar": true,
  "appUserModelIds": [
    "App User Model Ids value"
  ],
  "desktopAppPaths": [
    "Desktop App Paths value"
  ],
  "userAccounts": [
    "User Accounts value"
  ],
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 413

{
  "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
  "id": "cfa70299-0299-cfa7-9902-a7cf9902a7cf",
  "profileName": "Profile Name value",
  "showTaskBar": true,
  "appUserModelIds": [
    "App User Model Ids value"
  ],
  "desktopAppPaths": [
    "Desktop App Paths value"
  ],
  "userAccounts": [
    "User Accounts value"
  ],
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
}
```





