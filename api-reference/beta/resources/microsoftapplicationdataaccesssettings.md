---
title: Tipo de recurso microsoftApplicationDataAccessSettings
description: Representa configurações para determinar o acesso de aplicativos da Microsoft Microsoft 365 dados pertencentes aos usuários de uma organização. Por exemplo, dada a autorização adequada, se apenas aplicativos Microsoft 365 (como o Word e o Excel) podem acessar os dados Microsoft 365 dos usuários ou se outros aplicativos da Microsoft (como Windows) também podem acessar os dados.
author: ttomi
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 049089e4c3246beed9f459831cd7903dea9e4ce3
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589557"
---
# <a name="microsoftapplicationdataaccesssettings-resource-type"></a>Tipo de recurso microsoftApplicationDataAccessSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa _configurações que_ especificam o acesso de aplicativos Microsoft Microsoft 365 dados pertencentes aos usuários de uma organização. Por exemplo, dada a autorização adequada, se apenas aplicativos Microsoft 365 (como o Word e o Excel) podem acessar os dados Microsoft 365 dos usuários ou se outros aplicativos da Microsoft (como o Windows) também podem acessar os dados.

Exemplos de Microsoft 365 dados em uma organização incluem documentos do Word, Excel e PowerPoint, mensagens Outlook e gravações de reunião do Teams, para os quais o usuário no aplicativo Microsoft foi autorizado corretamente a acessar.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar microsoftApplicationDataAccessSettings](../api/organizationsettings-list-microsoftapplicationdataaccess.md)|[microsoftApplicationDataAccessSettings](microsoftapplicationdataaccesssettings.md)|Obter as _configurações_ em um [objeto microsoftApplicationDataAccessSettings](microsoftapplicationdataaccesssettings.md) que especificam o acesso de aplicativos Da Microsoft para Microsoft 365 dados do usuário em uma organização.|
|[Atualizar microsoftApplicationDataAccessSettings](../api/microsoftapplicationdataaccesssettings-update.md)|[microsoftApplicationDataAccessSettings](microsoftapplicationdataaccesssettings.md)|Atualize as configurações em um [objeto microsoftApplicationDataAccessSettings](microsoftapplicationdataaccesssettings.md) que especificam o acesso de aplicativos Microsoft para Microsoft 365 dados do usuário em uma organização.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isEnabledForAllMicrosoftApplications|Booliano|Quando definido como `true`, todos os usuários da organização podem acessar em um aplicativo microsoft qualquer Microsoft 365 dados que o usuário tenha sido autorizado a acessar. O aplicativo Da Microsoft pode ser um aplicativo Microsoft 365 (por exemplo, Excel, Outlook) ou aplicativo que não Microsoft 365 (por exemplo, Edge). O padrão é `true`. <br> É possível desabilitar esse acesso para um subconjunto de usuários em um grupo de segurança do Azure AD, especificando o grupo na **propriedade disabledForGroup** . <br> Quando definido como `false`, todos os usuários podem acessar dados Microsoft 365 autorizados somente em um Microsoft 365 aplicativo.|
|disabledForGroup|Cadeia de caracteres|A ID de um grupo de segurança do Azure Active Directory (Azure AD) para o qual os membros têm permissão para acessar dados Microsoft 365 usando apenas aplicativos Microsoft 365, mas não outros aplicativos da Microsoft, como o Edge. <br> Isso só será aplicável **se isEnabledForAllMicrosoftApplications** estiver definido como `true`.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.microsoftApplicationDataAccessSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftApplicationDataAccessSettings",
  "isEnabledForAllMicrosoftApplications": "Boolean",
  "disabledForGroup": "String"
}
```
