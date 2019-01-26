---
title: tipo de recurso de política
description: 'Representa uma política do Azure AD. Políticas são regras personalizadas que podem ser aplicadas em toda a organização atribuídos a eles, entidades de serviço, grupos ou aplicativos. Atualmente, somente um tipo de política está disponível:'
localization_priority: Normal
ms.openlocfilehash: bd946da13fc36925e284ad2af29585b37d0a9a3a
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576196"
---
# <a name="policy-resource-type"></a>tipo de recurso de política

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma política do Azure AD. Políticas são regras personalizadas que podem ser aplicadas em toda a organização atribuídos a eles, entidades de serviço, grupos ou aplicativos. Atualmente, somente um tipo de política está disponível:

- Política de tempo de vida de token - Especifica a duração de tempo de vida de tokens emitidos para aplicativos e entidades de serviço.

Esta diretiva é descrita em maiores detalhes a seguir.

## <a name="methods"></a>Métodos
| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
| [Obter diretiva](../api/policy-get.md) |Política|Ler propriedades e relações do objeto user.|
|[Criar política](../api/policy-post.md)|Política|Crie um novo objeto de diretiva.|
|[Política de atualização](../api/policy-update.md)|Nenhum|Objeto de diretiva de atualização.|
|[Excluir a diretiva](../api/policy-delete.md)|Nenhum|Exclua o objeto de diretiva.|
|[Atribuir política](../api/policy-assign.md)|Nenhum|Atribua uma política a um aplicativo, entidade de serviço.|
|[Lista de políticas](../api/policy-list.md)|Coleção de políticas|Obtenha todos os objetos de política na organização.|
|[Políticas de lista atribuída](../api/policy-list-assigned.md)|Coleção de políticas|Obtenha todos os objetos de política atribuídos a um aplicativo ou entidade de serviço.|

### <a name="common-properties"></a>Propriedades comuns
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|definição|String collection|A versão de cadeia de caracteres da diretiva específica. Veja a seguir. Obrigatório.|
|displayName|String|Um nome personalizado para a política. Obrigatório.|
|IsOrganizationDefault|Boolean|Se definido como verdadeiro, ativa essa diretiva. Pode haver várias políticas para o mesmo tipo de política, mas apenas um pode ser ativado como o padrão da organização. Opcional, valor padrão é false.|
|type|String|Especifica o tipo de política. No momento deve ser "TokenLifetimePolicy". Obrigatório.|

#### <a name="common-relationships"></a>Relações comuns
|Relação|Tipo|Descrição|
|:-------------|:-----------|:-----------|
|appliesTo|Coleção [directoryObject](../resources/directoryobject.md)|Os aplicativos, entidades de serviço, grupos ou organização a política se aplica.|

## <a name="token-lifetime-policy"></a>Política de vida útil do token
Especifica o tempo de vida de tokens emitidos para várias finalidades. Esse tipo de política pode ser [atribuído](../api/policy-assign.md) a aplicativos e entidades de serviço. Existem quatro tipos de tokens cujos tempos de vida podem ser configurados. Os pares de token de acesso/atualizar são obtidos durante a autenticação por meio de um cliente, enquanto os pares de token de ID/sessão são obtidos durante a autenticação por meio de um navegador.

- **Token de acesso** contém informações sobre a identidade e os privilégios associados a uma conta de usuário que é usada pelos clientes para acessar recursos protegidos como aplicativos.
- **Atualizar Token** é obtido junto com o token de acesso quando um usuário autenticado em Azure AD por meio de um cliente para acessar um recurso protegido. Enquanto não for revogado ou deixado não utilizado por mais do que o MaxInactiveTime (abaixo), ele pode ser usado para obter um novo par de token de acesso/atualizar quando expira o token de acesso atual.
- **ID do Token** se comporta como um token de acesso, mas obtidos por meio do navegador.
- **Token de sessão** se comporta como um token de atualização, mas obtido através do navegador.

## <a name="properties"></a>Propriedades
As propriedades abaixo o objeto JSON que representa uma política de vida útil do token de formulário. Este objeto JSON deve ser **convertido em uma cadeia de caracteres com cotações de escape** a ser inserido na propriedade de política comum "definição". Um exemplo é mostrado abaixo.

>Observação: Todas as durações de tempo nessas propriedades são especificadas no formato "dd".

>Observação: Os valores máximos para as propriedades denotados em "dias" são 1 segundo compara o número indicado de dias. Por exemplo, o valor máximo de dias 1 é especificado como "23: 59:59".

| Propriedade     | Tipo   |Descrição| Valor min | Valor max | Valor padrão|
|:---------------|:--------|:----------|:--------|:--------|:----|
|AccessTokenLifetime|String|Controla quanto tempo **acesso e tokens de ID** são considerados válidos.|10 minutos|1 dia|1 hora|
|MaxInactiveTime|String|Controla como antigo um token de atualização pode ser antes de um cliente não pode usá-lo para recuperar um novo par de token de acesso/atualizar para acessar um recurso.|10 minutos|90 dias|14 dias|
|MaxAgeSingleFactor|String|Controles quanto tempo um usuário pode continuar usando tokens de atualização para obter acesso/atualizar novo pares de tokens após a última vez em que eles autenticados com êxito com apenas um fator único. Porque o fator único é considerado menos seguro que a autenticação multifator, recomenda-se essa diretiva estiver definida como um valor igual ou menor que o MultiFactorRefreshTokenMaxAge.|10 minutos|até revogado|365 dias ou até revogado|
|MaxAgeMultiFactor|String|Controles quanto tempo um usuário pode continuar usando tokens de atualização para obter acesso/atualizar novo pares de tokens após a última vez em que eles autenticados com êxito com vários fatores.|10 minutos|até revogado|365 dias ou até revogado|
|MaxAgeSessionSingleFactor|String|Controles quanto tempo um usuário pode continuar usando tokens de sessão para obter tokens do novos ID/sessão após a última vez em que eles autenticado com sucesso com apenas um fator único. Como o fator único é considerado menos seguro que a autenticação multifator, é recomendável que essa diretiva estiver definida como um valor igual ou menor que o MultiFactorSessionTokenMaxAge|10 minutos|até revogado|365 ou até revogado|
|MaxAgeSessionMultiFactor|String|Controles quanto tempo um usuário pode continuar usando tokens de sessão para obter tokens do novos ID/sessão após a última vez em que eles autenticado com sucesso com vários fatores.|10 minutos|até revogado|365 ou até revogado|
|Versão|Inteiro|Defina o valor de 1. Obrigatório.|Nenhum|Nenhum|Nenhum|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.policy"
}-->

```json
{
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
  "displayName":"Test Policy",
  "isOrganizationDefault":false,
  "type":"TokenLifetimePolicy",
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/policy.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
