---
title: Tipo de recurso iosVppEBook
description: Uma classe que contém as propriedades do livro eletrônico Vpp iOS.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f3cdd76a86000fe2e5f755d0c8ed84c0d649de14
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086992"
---
# <a name="iosvppebook-resource-type"></a>Tipo de recurso iosVppEBook

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades do livro eletrônico Vpp iOS.


Herda de [managedEBook](../resources/intune-books-managedebook.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosVppEBooks](../api/intune-books-iosvppebook-list.md)|Coleção [iosVppEBook](../resources/intune-books-iosvppebook.md)|Lista propriedades e relações dos objetos [iosVppEBook](../resources/intune-books-iosvppebook.md).|
|[Obter iosVppEBook](../api/intune-books-iosvppebook-get.md)|[iosVppEBook](../resources/intune-books-iosvppebook.md)|Propriedades de leitura e relações do objeto [iosVppEBook](../resources/intune-books-iosvppebook.md).|
|[Criar iosVppEBook](../api/intune-books-iosvppebook-create.md)|[iosVppEBook](../resources/intune-books-iosvppebook.md)|Cria um novo objeto [iosVppEBook](../resources/intune-books-iosvppebook.md).|
|[Excluir iosVppEBook](../api/intune-books-iosvppebook-delete.md)|Nenhum|Exclui um [iosVppEBook](../resources/intune-books-iosvppebook.md).|
|[Atualizar iosVppEBook](../api/intune-books-iosvppebook-update.md)|[iosVppEBook](../resources/intune-books-iosvppebook.md)|Atualiza as propriedades de um objeto [iosVppEBook](../resources/intune-books-iosvppebook.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [managedEBook](../resources/intune-books-managedebook.md)|
|displayName|Cadeia de caracteres|Nome do livro eletrônico. Herdada de [managedEBook](../resources/intune-books-managedebook.md)|
|description|Cadeia de caracteres|Descrição. Herdada de [managedEBook](../resources/intune-books-managedebook.md)|
|publisher|Cadeia de caracteres|Publicador. Herdada de [managedEBook](../resources/intune-books-managedebook.md)|
|publishedDateTime|DateTimeOffset|A data e hora em que o livro eletrônico foi publicado. Herdada de [managedEBook](../resources/intune-books-managedebook.md)|
|largeCover|[mimeContent](../resources/intune-shared-mimecontent.md)|Capa do livro. Herdada de [managedEBook](../resources/intune-books-managedebook.md)|
|createdDateTime|DateTimeOffset|A data e hora em que o livro eletrônico foi modificado pela última vez. Herdada de [managedEBook](../resources/intune-books-managedebook.md)|
|lastModifiedDateTime|DateTimeOffset|A data e hora da última modificação do livro eletrônico. Herdada de [managedEBook](../resources/intune-books-managedebook.md)|
|informationUrl|String|A URL de informações adicionais. Herdada de [managedEBook](../resources/intune-books-managedebook.md)|
|privacyInformationUrl|String|A URL da declaração de privacidade. Herdada de [managedEBook](../resources/intune-books-managedebook.md)|
|vppTokenId|Guid|A ID de token Vpp.|
|appleId|Cadeia de caracteres|O Apple ID associado ao token Vpp.|
|vppOrganizationName|Cadeia de caracteres|O nome da organização do token Vpp.|
|genres|Coleção de cadeia de caracteres|Gêneros.|
|idioma|Cadeia de caracteres|Idioma.|
|seller|Cadeia de caracteres|Vendedor.|
|totalLicenseCount|Int32|Contagem total de licenças.|
|usedLicenseCount|Int32|Contagem de licenças usadas.|
|roleScopeTagIds|String collection|Lista de marcas de escopo para esta instância entity.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categories|[Coleção managedEBookCategory](../resources/intune-books-managedebookcategory.md)|A lista de categorias para este eBook. Herdada de [managedEBook](../resources/intune-books-managedebook.md)|
|assignments|Coleção [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)|A lista de atribuições para este livro eletrônico. Herdado de [managedEBook](../resources/intune-books-managedebook.md)|
|installSummary|[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md)|Resumo de instalação do aplicativo móvel. Herdado de [managedEBook](../resources/intune-books-managedebook.md)|
|deviceStates|Coleção [deviceInstallState](../resources/intune-books-deviceinstallstate.md)|A lista de estados de instalação para este livro eletrônico. Herdado de [managedEBook](../resources/intune-books-managedebook.md)|
|userStateSummary|Coleção [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)|A lista de estados de instalação para este livro eletrônico. Herdado de [managedEBook](../resources/intune-books-managedebook.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBook",
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
  "privacyInformationUrl": "String",
  "vppTokenId": "Guid",
  "appleId": "String",
  "vppOrganizationName": "String",
  "genres": [
    "String"
  ],
  "language": "String",
  "seller": "String",
  "totalLicenseCount": 1024,
  "usedLicenseCount": 1024,
  "roleScopeTagIds": [
    "String"
  ]
}
```



