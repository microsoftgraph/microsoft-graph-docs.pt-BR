---
title: Como clonar uma equipe
description: Crie uma cópia de uma equipe. Esta operação também cria uma cópia do grupo correspondente.
author: nkramer
ms.openlocfilehash: 79ae6f770e009f262adbda4872ddc51af626688f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361926"
---
# <a name="clone-a-team"></a>Como clonar uma equipe

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Crie uma cópia de uma [equipe](../resources/team.md). Esta operação também cria uma cópia do [grupo](../resources/group.md)correspondente.
Você pode especificar quais partes da equipe a ser clonada:

- **apps** - apps cópias equipes da Microsoft que estão instalados na equipe de. 
- **canais** – copia a estrutura de canal (mas não as mensagens no canal).
- **membros** – copia os membros e proprietários do grupo.
- **configurações** – copia todas as definições dentro da equipe, juntamente com as configurações de chave de grupo.
- **guias** – copia as guias no canais.

Quando as guias são clonados, eles são colocados em um estado não configurado- - são exibidas na barra de ferramentas guia da Microsoft Teams e, na primeira vez que você abri-los, vá através da tela de configuração. (Se a pessoa que está abrindo a guia não tem permissão para configurar os aplicativos, eles verão uma mensagem que explica que a guia ainda não foram configurada.)

A clonagem é uma operação de execução longa.
Depois que o clone POST retorna, você precisará fazer a [operação](../resources/teamsasyncoperation.md) para verificar se ele está "em execução" ou "sucedidas" ou "Falha". Você deve continuar GET até que o status não é "executando". O atraso recomendado entre obtém é 5 segundos.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | Group.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo                            | Group.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Corpo da solicitação

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|classificação|Cadeia de caracteres (opcional)|Descreve uma classificação para o grupo (por exemplo, o impacto comercial baixa, média ou alta). Os valores válidos para essa propriedade são definidos com a criação de um valor de [configuração](../resources/directorysetting.md) de ClassificationList, com base na [definição de modelo](../resources/directorysettingtemplate.md). Se a classificação não for especificada, a classificação será copiada do team/grupo original.|
|description|Cadeia de caracteres (opcional)|Uma descrição opcional para o grupo. Se essa propriedade não for especificada, ele será deixado em branco.|
|displayName|String|O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.|
|mailNickname|String|O alias de email para o grupo, exclusivo na organização. Esta propriedade deve ser especificada quando um grupo é criado. Oferece suporte a $filter. Se essa propriedade não for especificada, ele será calculado de displayName. Problema conhecido: esta propriedade é ignorada no momento.|
|partsToClone| [clonableTeamParts](../resources/clonableteamparts.md) |Uma lista separada por vírgulas das partes a ser clonada. Partes legais são "apps, guias, configurações, canais, membros".|
|visibilidade|[teamVisibilityType](../resources/teamvisibilitytype.md) (opcional)| Especifica a visibilidade do grupo. Os valores possíveis são: **particular**e **público**. Se a visibilidade não for especificada, será copiada a visibilidade do team/grupo original. Se a equipe que está sendo clonado é uma equipe **educationClass** , o parâmetro visibilidade será ignorado e visibilidade do novo grupo será definida como HiddenMembership.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `202 Accepted` código de resposta com um local: cabeçalho apontando para o recurso de [operação](../resources/teamsasyncoperation.md) .
Quando a operação for concluída, o recurso de operação informará a id da equipe de criação.

## <a name="example"></a>Exemplo
#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.
<!-- {
  "blockType": "ignored",
  "name": "create_team"
}-->
```http
POST /teams/{id}/clone
Content-Type: application/json

{  
     "displayName": "Library Assist",
     "description": "Self help community for library",
     "mailNickname": "libassist",
     "partsToClone": "apps,tabs,settings,channels,members",
     "visibility": "public"
}
```

#### <a name="response"></a>Resposta
Este é um exemplo de resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
