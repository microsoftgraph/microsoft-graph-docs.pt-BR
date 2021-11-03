---
title: Tipo de recurso federatedIdentityCredential
description: Faz referência às credenciais de identidade federada de um aplicativo. Essas credenciais de identidade federadas são usadas na federação de identidade de carga de trabalho ao trocar um token de um emissor confiável por um token de acesso vinculado a um aplicativo registrado no Azure AD.
author: kjyam98
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: fb5d51cd16103c21656927b999bf5484d70d0800
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697175"
---
# <a name="federatedidentitycredential-resource-type"></a>Tipo de recurso federatedIdentityCredential

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Faz referência às credenciais de identidade federada de um aplicativo. Essas credenciais de identidade federadas são usadas na federação de identidade de carga de trabalho ao trocar um token de um emissor confiável por um token de acesso vinculado a um aplicativo registrado no Azure AD. [](/azure/active-directory/develop/workload-identity-federation)

Herda da [entidade](../resources/entity.md).

>**OBSERVAÇÃO:** Esse recurso não está disponível em [implantações de nuvem](/graph/deployments) nacionais.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar federatedIdentityCredentials](../api/application-list-federatedidentitycredentials.md)|[Coleção federatedIdentityCredential](../resources/federatedidentitycredential.md)|Obter uma lista dos [objetos federatedIdentityCredential](../resources/federatedidentitycredential.md) e suas propriedades.|
|[Criar federatedIdentityCredential](../api/application-post-federatedidentitycredentials.md)|[federatedIdentityCredential](../resources/federatedidentitycredential.md)|Crie um novo [objeto federatedIdentityCredential.](../resources/federatedidentitycredential.md)|
|[Obter federatedIdentityCredential](../api/federatedidentitycredential-get.md)|[federatedIdentityCredential](../resources/federatedidentitycredential.md)|Leia as propriedades e as relações de um [objeto federatedIdentityCredential.](../resources/federatedidentitycredential.md)|
|[Atualizar federatedIdentityCredential](../api/federatedidentitycredential-update.md)|Nenhum|Atualize as propriedades de um [objeto federatedIdentityCredential.](../resources/federatedidentitycredential.md)|
|[Excluir federatedIdentityCredential](../api/federatedidentitycredential-delete.md)|Nenhum|Exclui um [objeto federatedIdentityCredential.](../resources/federatedidentitycredential.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| audiences | Coleção de cadeias de caracteres | Lista as audiências que podem aparecer no token externo. Esse campo é obrigatório e é padrão para "api://AzureADTokenExchange". Ele diz o plataforma de identidade da Microsoft deve aceitar na `aud` declaração no token de entrada. Esse valor representa o Azure AD em seu provedor de identidade externo e não tem valor fixo entre provedores de identidade - talvez seja necessário criar um novo registro de aplicativo em seu provedor de identidade para servir como audiência desse token. Obrigatório. |
| description | String | A descrição não validada e fornecida pelo usuário da credencial de identidade federada. Opcional.  |
| id| String | O identificador exclusivo da identidade federada. Obrigatório. Apenas leitura.  |
| emissor | String | A URL do provedor de identidade externa e deve corresponder à `issuer` declaração do token externo que está sendo trocado. A combinação dos valores de **emissor** e **assunto** deve ser exclusiva no aplicativo. Obrigatório. |
| name | String | é o identificador exclusivo da credencial de identidade federada, que tem um limite de caracteres de 120 caracteres e deve ser amigável à URL. Ele é imutável uma vez criado. Obrigatório. Não anulável. Suporta `$filter` (`eq`). |
| assunto | String | Obrigatório. O identificador da carga de trabalho de software externo no provedor de identidade externa. Como o valor da audiência, ele não tem formato fixo, pois cada provedor de identidade usa seu próprio - às vezes um GUID, às vezes um identificador delimitado por dois pontos, às vezes cadeias de caracteres arbitrárias. O valor aqui deve corresponder à `sub` declaração dentro do token apresentado ao Azure AD. A combinação de **emissor e** **assunto** deve ser exclusiva no aplicativo. Suporta `$filter` (`eq`). |


## <a name="relationships"></a>Relações

Nenhum


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.federatedIdentityCredential",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.federatedIdentityCredential",
  "name": "String",
  "issuer": "String",
  "subject": "String",
  "description": "String",
  "audiences": [
    "String"
  ]
}
```

