---
title: Tipo de recurso mobileAppContent
description: Contém propriedades de conteúdo para uma versão específica do aplicativo. Cada mobileAppContent pode ter vários mobileAppContentFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c36a306e0b594ff84bffbc3e80fd393d20051371
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759006"
---
# <a name="mobileappcontent-resource-type"></a>Tipo de recurso mobileAppContent

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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
|id|String|A versão do conteúdo do aplicativo.|

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




