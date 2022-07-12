---
title: Tipo de recurso macOSOfficeSuiteApp
description: Contém propriedades e propriedades herdadas do aplicativo do MacOS Office Suite.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3242ce8b8db4b0ca7d9c7891095339589411c37a
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66731033"
---
# <a name="macosofficesuiteapp-resource-type"></a>Tipo de recurso macOSOfficeSuiteApp

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades e propriedades herdadas do aplicativo do MacOS Office Suite.


Herda de [mobileApp](../resources/intune-apps-mobileapp.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar macOSOfficeSuiteApps](../api/intune-apps-macosofficesuiteapp-list.md)|Coleção [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md)|Lista propriedades e relações dos objetos [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).|
|[Obter macOSOfficeSuiteApp](../api/intune-apps-macosofficesuiteapp-get.md)|[macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md)|Propriedades de leitura e relações do objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).|
|[Criar macOSOfficeSuiteApp](../api/intune-apps-macosofficesuiteapp-create.md)|[macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md)|Cria um novo objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).|
|[Excluir macOSOfficeSuiteApp](../api/intune-apps-macosofficesuiteapp-delete.md)|Nenhum|Exclui um [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).|
|[Atualizar macOSOfficeSuiteApp](../api/intune-apps-macosofficesuiteapp-update.md)|[macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md)|Atualiza as propriedades de um objeto [ macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|displayName|String|O título do aplicativo importado ou definido pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|description|String|A descrição do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|publicador|String|O publicador do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|createdDateTime|DateTimeOffset|A data e a hora da criação do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora que o aplicativo foi modificado pela última vez. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|isFeatured|Boolean|O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|privacyInformationUrl|String|A URL da declaração de privacidade. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|informationUrl|String|A URL de informações adicionais. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|owner|String|O proprietário do conteúdo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|developer|String|O desenvolvedor do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|notes|String|Anotações do aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|publishingState|[mobileAppPublishingState](../resources/intune-apps-mobileapppublishingstate.md)|O estado de publicação do aplicativo. O aplicativo não pode ser assinado, a menos que ele seja publicado. Herdado do [mobileApp](../resources/intune-apps-mobileapp.md). Os valores possíveis são: `notPublished`, `processing`, `published`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categories|Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|A lista de categorias para este aplicativo. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|
|assignments|Coleção [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)|A lista de atribuições de grupo para esse aplicativo móvel. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSOfficeSuiteApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "publishingState": "String"
}
```





