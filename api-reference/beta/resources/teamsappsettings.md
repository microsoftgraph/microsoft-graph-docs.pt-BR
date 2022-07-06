---
title: Tipo de recurso teamsAppSettings
description: Representa as configurações de aplicativo do Teams
author: subray2014
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0a36f6657dc8231450514eb6c60d7d729c0e0818
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645596"
---
# <a name="teamsappsettings-resource-type"></a>Tipo de recurso teamsAppSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa configurações de todo o locatário para todos os [aplicativos do Teams](teamsapp.md) no locatário.

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter teamsAppSettings](../api/teamsappsettings-get.md)|[teamsAppSettings](../resources/teamsappsettings.md)|Obtenha as configurações de todo o locatário para todos os aplicativos do Teams no locatário.|
|[Atualizar teamsAppSettings](../api/teamsappsettings-update.md)|[teamsAppSettings](../resources/teamsappsettings.md)|Atualize as configurações de todo o locatário para todos os aplicativos do Teams no locatário.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isChatResourceSpecificConsentEnabled|Booleano|Indica se o consentimento específico do recurso para chats/reuniões foi habilitado para o locatário. Se verdadeiro, os aplicativos do Teams permitidos no locatário e que exigem permissões específicas de recursos podem ser instalados dentro de chats e reuniões. Se for false, a instalação de qualquer aplicativo do Teams que exija permissões específicas de recursos em um chat ou reunião será bloqueada.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsAppSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsAppSettings",
  "id": "String (identifier)",
  "isChatResourceSpecificConsentEnabled": "Boolean"
}
```

## <a name="see-also"></a>Confira também

- [Consentimento específico do recurso](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)