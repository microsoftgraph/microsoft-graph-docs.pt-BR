---
title: tipo de recurso userAccountInformation
description: tipo de recurso userAccountInformation
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a633b6de9269b67fcf26dea035438a3494c4515c
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812741"
---
# <a name="useraccountinformation-resource-type"></a>tipo de recurso userAccountInformation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações especificamente ligadas à conta de um usuário, seja ela uma conta do Azure AD ou uma conta da Microsoft. O identificador de entidade é definido como o GUID do Azure AD correspondente ou o CID da conta da Microsoft, respectivamente. Esses campos são somente leitura por meio do Microsoft Graph e devem ser editados por meio de um perfil de usuário ou por um administrador de locatários em uma experiência correspondente.

Herda de [Myfacet](itemfacet.md).

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar contas](../api/profile-list-accounts.md)|coleção [userAccountInformation](../resources/useraccountinformation.md)|Obtenha os recursos userAccountInformation da propriedade de navegação Account.|
|[Criar userAccountInformation](../api/profile-post-accounts.md)|[userAccountInformation](../resources/useraccountinformation.md)|Criar um novo objeto userAccountInformation.|
|[Obter userAccountInformation](../api/useraccountinformation-get.md)|[userAccountInformation](../resources/useraccountinformation.md)|Leia as propriedades e os relacionamentos de um objeto [userAccountInformation](../resources/useraccountinformation.md) .|
|[Atualizar userAccountInformation](../api/useraccountinformation-update.md)|[userAccountInformation](../resources/useraccountinformation.md)|Atualiza as propriedades de um objeto [userAccountInformation](../resources/useraccountinformation.md) .|
|[Excluir userAccountInformation](../api/useraccountinformation-delete.md)|Nenhum|Exclui um objeto [userAccountInformation](../resources/useraccountinformation.md) .|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ageGroup|String|Mostra o grupo de idade do usuário. Os valores `null` permitidos `minor` , `notAdult` e `adult` são gerados pelo diretório e não podem ser alterados.|
|allowedAudiences|String|As audiências que podem ver os valores contidos na entidade. Herdado de [MyFace](../resources/itemfacet.md). Os valores possíveis são: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|countryCode|String|Contém o código de país de dois caracteres associado à conta de usuários.  |
|createdBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que criou a entidade. Herdado de [MyFace](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|id|String|Identificador usado para o endereçamento individual da entidade. Herdado da [entidade](../resources/entity.md)|
|fracassa|[inferenceData](../resources/inferencedata.md)|Contém detalhes de inferência se a entidade for inferida pelo aplicativo de criação ou modificação. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Fornece o identificador do usuário e/ou aplicativo que modificou a entidade pela última vez. Herdado de [MyFace](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Fornece o dateTimeOffset para quando a entidade foi criada. Herdado de [MyFace](../resources/itemfacet.md).|
|preferredLanguageTag|[localeInfo](../resources/localeinfo.md)|Contém o idioma que o usuário associou como preferencial para a conta.   |
|source|[personDataSource](../resources/persondatasource.md)|Onde os valores são originados se forem sincronizados a partir de outro serviço. Herdado de [MyFace](../resources/itemfacet.md).|
|userPrincipalName|String|O nome principal do usuário (UPN) do usuário associado à conta.   |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userAccountInformation",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userAccountInformation",
  "id": "String (identifier)",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  },
  "ageGroup": "String",
  "countryCode": "String",
  "preferredLanguageTag": {
    "@odata.type": "microsoft.graph.localeInfo"
  },
  "userPrincipalName": "String"
}
```
