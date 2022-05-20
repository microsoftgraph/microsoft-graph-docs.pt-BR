---
title: Tipo de recurso federatedIdentityCredential
description: Faz referência às credenciais de identidade federada de um aplicativo. Essas credenciais de identidade federada são usadas na federação de identidade de carga de trabalho ao trocar um token de um emissor confiável por um token de acesso vinculado a um aplicativo registrado no Azure AD.
author: shahzad-khalid
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 4a529d1079c3058a1cb381e8b46c7849d8d4f3dd
ms.sourcegitcommit: 995056279c2151d7ce4a0fcff067fbc6edced728
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2022
ms.locfileid: "65602739"
---
# <a name="federatedidentitycredential-resource-type"></a>Tipo de recurso federatedIdentityCredential

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Faz referência às credenciais de identidade federada de um aplicativo. Essas credenciais de identidade federada são usadas [](/azure/active-directory/develop/workload-identity-federation) na federação de identidade de carga de trabalho ao trocar um token de um emissor confiável por um token de acesso vinculado a um aplicativo registrado no Azure AD.

Herda de [entidade](../resources/entity.md).

>**NOTA:** Esse recurso não está disponível em [implantações de nuvem](/graph/deployments) nacional.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar federatedIdentityCredentials](../api/application-list-federatedidentitycredentials.md)|Coleção [federatedIdentityCredential](../resources/federatedidentitycredential.md)|Obtenha uma lista dos objetos [federatedIdentityCredential](../resources/federatedidentitycredential.md) e suas propriedades.|
|[Criar federatedIdentityCredential](../api/application-post-federatedidentitycredentials.md)|[federatedIdentityCredential](../resources/federatedidentitycredential.md)|Crie um novo [objeto federatedIdentityCredential](../resources/federatedidentitycredential.md) .|
|[Obter federatedIdentityCredential](../api/federatedidentitycredential-get.md)|[federatedIdentityCredential](../resources/federatedidentitycredential.md)|Leia as propriedades e as relações de um [objeto federatedIdentityCredential](../resources/federatedidentitycredential.md) .|
|[Atualizar federatedIdentityCredential](../api/federatedidentitycredential-update.md)|Nenhum|Atualize as propriedades de um [objeto federatedIdentityCredential](../resources/federatedidentitycredential.md) .|
|[Excluir federatedIdentityCredential](../api/federatedidentitycredential-delete.md)|Nenhum|Exclui um [objeto federatedIdentityCredential](../resources/federatedidentitycredential.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| Público | Coleção de cadeias de caracteres | Lista as audiências que podem aparecer no token externo. Esse campo é obrigatório e usa como padrão "api://AzureADTokenExchange". Ele diz o plataforma de identidade da Microsoft deve aceitar na declaração `aud` no token de entrada. Esse valor representa Azure AD em seu provedor de identidade externo e não tem nenhum valor fixo entre provedores de identidade – talvez seja necessário criar um novo registro de aplicativo em seu provedor de identidade para servir como o público-alvo desse token. Obrigatório. |
| description | Cadeia de caracteres | A descrição não validada fornecida pelo usuário da credencial de identidade federada. Opcional.  |
| id| Cadeia de caracteres | O identificador exclusivo da identidade federada. Obrigatório. Somente leitura.  |
| Emissor | Cadeia de caracteres | A URL do provedor de identidade externa e deve corresponder à `issuer` declaração do token externo que está sendo trocado. A combinação dos valores do **emissor e** **da entidade** deve ser exclusiva no aplicativo. Obrigatório. |
| nome | String | é o identificador exclusivo para a credencial de identidade federada, que tem um limite de caracteres de 120 caracteres e deve ser amigável para URL. Ele é imutável depois de criado. Obrigatório. Não anulável. Suporta `$filter` (`eq`). |
| assunto | Cadeia de caracteres | Obrigatório. O identificador da carga de trabalho de software externo no provedor de identidade externo. Como o valor do público-alvo, ele não tem nenhum formato fixo, pois cada provedor de identidade usa seu próprio – às vezes, um GUID, às vezes um identificador delimitado por dois-pontos, às vezes cadeias de caracteres arbitrárias. O valor aqui deve corresponder à declaração `sub` dentro do token apresentado a Azure AD. A combinação de **emissor e** **assunto** deve ser exclusiva no aplicativo. Suporta `$filter` (`eq`). |


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

