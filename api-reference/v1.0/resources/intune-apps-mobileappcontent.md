---
title: Tipo de recurso mobileAppContent
description: Contém propriedades de conteúdo para uma versão específica do aplicativo. Cada mobileAppContent pode ter vários mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9cde82585bdbe4ca4c15102e6b343810f29fdae8
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261296"
---
# <a name="mobileappcontent-resource-type"></a>Tipo de recurso mobileAppContent

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades de conteúdo para uma versão específica do aplicativo. Cada mobileAppContent pode ter vários mobileAppContentFile.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileAppContents](../api/intune-apps-mobileappcontent-list.md)|Conjunto [mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Listar propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).|
|[Obter mobileAppContent](../api/intune-apps-mobileappcontent-get.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Ler propriedades e relações de objetos de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).|
|[Criar mobileAppContent](../api/intune-apps-mobileappcontent-create.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Criar um novo objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).|
|[Excluir mobileAppContent](../api/intune-apps-mobileappcontent-delete.md)|Nenhum|Excluir [mobileAppContent](../resources/intune-apps-mobileappcontent.md).|
|[Atualizar mobileAppContent](../api/intune-apps-mobileappcontent-update.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|Atualizar as propriedades de um objeto de [mobileAppContent](../resources/intune-apps-mobileappcontent.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A versão do conteúdo do aplicativo.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|arquivos|Conjunto [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)|A lista dos arquivos desta versão de conteúdo do aplicativo.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```



