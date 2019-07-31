---
title: tipo de recurso de política
description: 'Representa uma política do Azure AD. As políticas são regras personalizadas que podem ser aplicadas em aplicativos, entidades de serviço, grupos ou toda a organização à qual foram atribuídas. Atualmente, somente um tipo de política está disponível:'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4a97caf82a53900ac4ba1e81cebddda114336597
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965807"
---
# <a name="policy-resource-type"></a>tipo de recurso de política

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política do Azure AD. As políticas são regras personalizadas que podem ser aplicadas em aplicativos, entidades de serviço, grupos ou toda a organização à qual foram atribuídas. Atualmente, somente um tipo de política está disponível:

- Política de tempo de vida do token – especifica o tempo de vida útil dos tokens emitidos para aplicativos e entidades de serviço.

Essa política é descrita em mais detalhes abaixo.

## <a name="methods"></a>Métodos
| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
| [Obter política](../api/policy-get.md) |Política|Ler propriedades e relações do objeto user.|
|[Criar uma política](../api/policy-post.md)|Política|Criar um novo objeto de política.|
|[Atualizar política](../api/policy-update.md)|Nenhum|Atualize o objeto Policy.|
|[Excluir política](../api/policy-delete.md)|Nenhum|Exclua o objeto Policy.|
|[Atribuir política](../api/policy-assign.md)|Nenhum|Atribuir uma política a um aplicativo, entidade de serviço.|
|[Listar políticas](../api/policy-list.md)|Coleção Policy|Obter todos os objetos de política na organização.|
|[Listar políticas atribuídas](../api/policy-list-assigned.md)|Coleção Policy|Obter todos os objetos de política atribuídos a uma entidade de serviço ou aplicativo.|

##  <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|definir|Coleção de cadeias de caracteres|A versão de cadeia de caracteres da política específica. Confira a seguir. Obrigatório.|
|displayName|String|Um nome personalizado para a política. Obrigatório.|
|IsOrganizationDefault|Booliano|Se definido como true, ativa esta política. Pode haver muitas políticas para o mesmo tipo de política, mas apenas uma pode ser ativada como a organização padrão. Opcional, o valor padrão é false.|
|type|String|Especifica o tipo de política. No momento, deve ser "TokenLifetimePolicy". Obrigatório.|
|alternativeIdentifer|String| |
|keyCredentials| Coleção [keyCredential](keycredential.md)| |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.policy",
  "keyProperty": "id",
  "baseType":"microsoft.graph.directoryObject",  
  "openType": true
}-->
```json
{
  "alternativeIdentifer": "String",
  "definition": ["String"],
  "displayName": "String",
  "isOrganizationDefault": "Boolean",
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "type": "String"
}
```

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:-------------|:-----------|:-----------|
|appliesTo|Coleção [directoryObject](../resources/directoryobject.md)|Os aplicativos, entidades de serviço, grupos ou organizações aos quais a política se aplica.|

### <a name="token-lifetime-policy"></a>Política do tempo de vida do token
Especifica os tempos de vida dos tokens emitidos para várias finalidades. Esse tipo de política pode ser [atribuído](../api/policy-assign.md) a aplicativos e entidades de serviço. Há quatro tipos de tokens cuja vida útil pode ser configurada. Os pares de tokens de acesso/atualização são obtidos durante a autenticação por meio de um cliente, enquanto os pares de identificador/sessão de ID são obtidos durante a autenticação por meio de um navegador.

- O **token de acesso** contém informações sobre a identidade e os privilégios associados a uma conta de usuário usada por clientes para acessar recursos protegidos, como aplicativos.
- O **token de atualização** é obtido junto com o token de acesso quando um usuário se autentica no Azure ad por meio de um cliente para acessar um recurso protegido. Apesar de não ser revogado ou não ser usado mais do que o MaxInactiveTime (abaixo), ele pode ser usado para obter um novo par de tokens de acesso/atualização quando o token de acesso atual expirar.
- O **token de ID** se comporta como um token de acesso, mas obtido através do navegador.
- O **token de sessão** se comporta como um token de atualização, mas obtido através do navegador.

#### <a name="properties-of-a-token-lifetime-policy"></a>Propriedades de uma política de tempo de vida do token
As propriedades abaixo formam o objeto JSON que representa uma política de tempo de vida do token. Esse objeto JSON deve ser **convertido em uma cadeia de caracteres com aspas de escape** a ser inserido na propriedade de política comum "definição". Um exemplo é mostrado abaixo no formato JSON:

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"
  ]
```

>Observação: todas as durações de tempo nessas propriedades são especificadas no formato "dd. hh: mm: SS".

>Observação: os valores máximos para propriedades denotadas em "dias" são 1 segundo curto do número de dias indicado. Por exemplo, o valor máximo de 1 dia é especificado como "23:59:59".

| Propriedade     | Tipo   |Descrição| Valor mínimo | Valor máximo | Valor padrão|
|:---------------|:--------|:----------|:--------|:--------|:----|
|AccessTokenLifetime|String|Controla por quanto tempo **os tokens de acesso e de ID** são considerados válidos.|10 minutos|1 dia|1 hour|
|MaxInactiveTime|String|Controla como o antigo token de atualização pode ser antes que um cliente não possa mais usá-lo para recuperar um novo par de tokens de acesso/atualização para acessar um recurso.|10 minutos|90 dias|14 dias|
|MaxAgeSingleFactor|String|Controla por quanto tempo um usuário pode continuar a usar tokens de atualização para obter novos pares de tokens de acesso/atualização após a última vez que autenticar com êxito apenas um único fator. Como o fator único é considerado menos seguro do que a autenticação multifator, é recomendável que essa política seja definida como um valor igual ou menor do que o MultiFactorRefreshTokenMaxAge.|10 minutos|até a revogação|365 dias ou até-revogados|
|MaxAgeMultiFactor|String|Controla por quanto tempo um usuário pode continuar a usar os tokens de atualização para obter novos pares de tokens de acesso/atualização após a última vez em que foram autenticados com vários fatores.|10 minutos|até a revogação|365 dias ou até-revogados|
|MaxAgeSessionSingleFactor|String|Controla por quanto tempo um usuário pode continuar a usar tokens de sessão para obter novos tokens de ID/sessão após a última vez que eles forem autenticados com êxito apenas com um único fator. Como o fator único é considerado menos seguro do que a autenticação multifator, é recomendável que essa política seja definida como um valor igual ou menor do que o MultiFactorSessionTokenMaxAge|10 minutos|até a revogação|365 ou até-revogado|
|MaxAgeSessionMultiFactor|String|Controla por quanto tempo um usuário pode continuar a usar tokens de sessão para obter novos tokens de sessão/ID após a última vez em que foram autenticados com vários fatores.|10 minutos|até a revogação|365 ou até-revogado|
|Versão|Inteiro|Defina o valor 1. Obrigatório.|Nenhum|Nenhum|Nenhum|


