---
title: Tipo de recurso managedEBook
description: Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3e1c4513c824ceb52f9036a1cdb847277fdca548
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66732433"
---
# <a name="managedebook-resource-type"></a>Tipo de recurso managedEBook

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedEBooks](../api/intune-books-managedebook-list.md)|Coleção [managedEBook](../resources/intune-books-managedebook.md)|Lista propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).|
|[Obter managedEBook](../api/intune-books-managedebook-get.md)|[managedEBook](../resources/intune-books-managedebook.md)|Propriedades de leitura e relações do objeto [managedEBook](../resources/intune-books-managedebook.md).|
|[ação assign](../api/intune-books-managedebook-assign.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|displayName|String|Nome do livro eletrônico.|
|description|String|Descrição.|
|publisher|Cadeia de caracteres|Publicador.|
|publishedDateTime|DateTimeOffset|A data e hora em que o livro eletrônico foi publicado.|
|largeCover|[mimeContent](../resources/intune-shared-mimecontent.md)|Capa do livro.|
|createdDateTime|DateTimeOffset|A data e hora em que o livro eletrônico foi modificado pela última vez.|
|lastModifiedDateTime|DateTimeOffset|A data e hora da última modificação do livro eletrônico.|
|informationUrl|String|A URL de informações adicionais.|
|privacyInformationUrl|String|A URL da declaração de privacidade.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|A lista de atribuições para este livro eletrônico.|
|installSummary|[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)|Resumo de instalação do aplicativo móvel.|
|deviceStates|Coleção [deviceInstallState](../resources/intune-books-deviceinstallstate.md)|A lista de estados de instalação para este livro eletrônico.|
|userStateSummary|Coleção [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)|A lista de estados de instalação para este livro eletrônico.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```





