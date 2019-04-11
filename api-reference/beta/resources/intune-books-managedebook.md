---
title: Tipo de recurso managedEBook
description: Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 888df51e17ab45dcada3d69fad95315b26b4b20e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31800396"
---
# <a name="managedebook-resource-type"></a>Tipo de recurso managedEBook

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe abstrata que contém as propriedades base do livro eletrônico gerenciado.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedEBooks](../api/intune-books-managedebook-list.md)|Coleção [managedEBook](../resources/intune-books-managedebook.md)|Lista propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).|
|[Acessar managedEBook](../api/intune-books-managedebook-get.md)|[managedEBook](../resources/intune-books-managedebook.md)|Leia as propriedades e as relações do objeto [managedEBook](../resources/intune-books-managedebook.md).|
|[atribuir ação](../api/intune-books-managedebook-assign.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|displayName|Cadeia de caracteres|Nome do livro eletrônico.|
|description|String|Descrição.|
|publisher|Cadeia de caracteres|Publicador.|
|publishedDateTime|DateTimeOffset|A data e hora em que o livro eletrônico foi publicado.|
|largeCover|[mimeContent](../resources/intune-shared-mimecontent.md)|Capa do livro.|
|createdDateTime|DateTimeOffset|A data e hora em que o livro eletrônico foi modificado pela última vez.|
|lastModifiedDateTime|DateTimeOffset|A data e hora da última modificação do livro eletrônico.|
|informationUrl|String|A URL de informações adicionais.|
|privacyInformationUrl|Cadeia de caracteres|A URL da declaração de privacidade.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categories|coleção [managedEBookCategory](../resources/intune-books-managedebookcategory.md)|A lista de categorias para este eBook.|
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





