---
title: Tipo de recurso iosVppEBook
description: Uma classe que contém as propriedades do livro eletrônico Vpp iOS.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 74f2f71b9f6f31e2574afb16c276ba42fb87c9a8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930233"
---
# <a name="iosvppebook-resource-type"></a>Tipo de recurso iosVppEBook

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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
|id|Cadeia de caracteres|Chave da entidade. Herdado de [managedEBook](../resources/intune-books-managedebook.md)|
|displayName|Cadeia de caracteres|Nome do livro eletrônico. Herdado de [managedEBook](../resources/intune-books-managedebook.md)|
|descrição|Cadeia de caracteres|Descrição. Herdado de [managedEBook](../resources/intune-books-managedebook.md)|
|publisher|Cadeia de caracteres|Publicador. Herdado de [managedEBook](../resources/intune-books-managedebook.md)|
|publishedDateTime|DateTimeOffset|A data e hora em que o livro eletrônico foi publicado. Herdado de [managedEBook](../resources/intune-books-managedebook.md)|
|largeCover|[mimeContent](../resources/intune-shared-mimecontent.md)|Capa do livro. Herdado de [managedEBook](../resources/intune-books-managedebook.md)|
|createdDateTime|DateTimeOffset|A data e hora em que o livro eletrônico foi modificado pela última vez. Herdado de [managedEBook](../resources/intune-books-managedebook.md)|
|lastModifiedDateTime|DateTimeOffset|A data e hora da última modificação do livro eletrônico. Herdada de [managedEBook](../resources/intune-books-managedebook.md)|
|informationUrl|Cadeia de caracteres|A URL de informações adicionais. Herdado de [managedEBook](../resources/intune-books-managedebook.md)|
|privacyInformationUrl|Cadeia de caracteres|A URL da declaração de privacidade. Herdado de [managedEBook](../resources/intune-books-managedebook.md)|
|vppTokenId|Guid|A ID de token Vpp.|
|appleId|Cadeia de caracteres|O Apple ID associado ao token Vpp.|
|vppOrganizationName|Cadeia de caracteres|O nome da organização do token Vpp.|
|genres|Coleção de cadeias de caracteres|Gêneros.|
|idioma|Cadeia de caracteres|Idioma.|
|seller|Cadeia de caracteres|Vendedor.|
|totalLicenseCount|Int32|Contagem total de licenças.|
|usedLicenseCount|Int32|Contagem de licenças usadas.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|categories|coleção [managedEBookCategory](../resources/intune-books-managedebookcategory.md)|A lista de categorias para este livro eletrônico. Herdado de [managedEBook](../resources/intune-books-managedebook.md)|
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
  "usedLicenseCount": 1024
}
```





