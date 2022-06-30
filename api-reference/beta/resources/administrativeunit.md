---
title: Tipo de recurso administrativeUnit
description: Uma unidade administrativa fornece um contêiner conceitual para objetos de diretório usuário e grupo.
ms.localizationpriority: medium
author: DougKirschner
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 702ff256e52721af990ee0fc211b4178dc0ad972
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555496"
---
# <a name="administrativeunit-resource-type"></a>Tipo de recurso administrativeUnit

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma unidade administrativa fornece um contêiner conceitual para objetos de diretório de usuário, grupo e dispositivo. Usando unidades administrativas, um administrador da empresa agora pode delegar responsabilidades administrativas para gerenciar os usuários, grupos e dispositivos contidos dentro ou no escopo de uma unidade administrativa para um administrador regional ou departamento. Esse recurso é um tipo aberto que permite que outras propriedades sejam passadas.

Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/administrativeunit-delta.md). 

Vejamos um exemplo. Imagine que a Contoso Corp é composta por duas divisões: uma Divisão da Costa Oeste e uma Divisão da Costa Leste. As funções de diretório na Contoso têm como escopo todo o locatário. Lee, um administrador da empresa Contoso, deseja delegar responsabilidades administrativas, mas defina-as como escopo para a Divisão da Costa Oeste ou para a divisão da Costa Leste.  Lee pode criar uma *unidade admistrativa* da Costa Oeste e colocar todos os usuários da Costa Oeste nessa unidade administrativa.  Da mesma forma, Lee pode criar uma *unidade administrativa da Costa Leste*.  Agora Lee, pode começar a delegar responsabilidades administrativas a outras  pessoas, mas com escopo para as novas unidades administrativas que ele criou. Lee coloca Jennifer em uma *função de* administrador de assistência **técnica com** escopo para a *unidade administrativa da Costa Oeste*.  Isso permite que Jennifer redefina a senha de qualquer usuário, mas somente se esses usuários estão na *unidade administrativa da Costa Oeste*.  Da mesma forma, Lee coloca Dave em uma função de administrador de *conta* de **usuário** com escopo para a *unidade administrativa da Costa Leste*.  Isso permite que Dave atualize usuários, atribua licenças e redefina a senha de qualquer usuário, mas somente se esses usuários estão na unidade administrativa *da Costa Leste*. Para obter uma visão geral em vídeo, consulte [Introdução às Unidades Administrativas do Azure Active Directory](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units).

Esse recurso permite:

- Adicionar seus próprios dados às propriedades personalizadas como [extensions](/graph/extensibility-overview).
- Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/user-delta.md).


## <a name="methods"></a>Métodos

| Método   | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Criar](../api/directory-post-administrativeunits.md) | [administrativeUnit](administrativeunit.md) | Crie uma nova unidade administrativa.|
|[Lista](../api/directory-list-administrativeunits.md) | [coleção administrativeUnit](administrativeunit.md) |Listar propriedades de todas as administrativeUnits.|
|[Get](../api/administrativeunit-get.md) | [administrativeUnit](administrativeunit.md) |Ler propriedades e relações de um objeto administrativeUnit específico.|
|[Atualizar](../api/administrativeunit-update.md) | [administrativeUnit](administrativeunit.md)    |Atualize o objeto administrativeUnit. |
|[Excluir](../api/administrativeunit-delete.md) | Nenhum |Exclua o objeto administrativeUnit. |
|[Obter delta](../api/administrativeunit-delta.md)|[administrativeUnit](administrativeunit.md)|Obtenha **administrativeUnits** recém-criados, atualizados ou excluídos sem precisar executar uma leitura completa de toda a coleção de recursos.|
|[Adicionar um membro](../api/administrativeunit-post-members.md) |[directoryObject](directoryobject.md)| Adicionar um membro (usuário ou grupo).|
|[Listar membros](../api/administrativeunit-list-members.md) |Coleção [directoryObject](directoryobject.md)| Obtenha a lista de membros (usuário e grupo).|
|[Obter um membro](../api/administrativeunit-get-members.md) |[directoryObject](directoryobject.md)| Obter um membro específico.|
|[Remover um membro](../api/administrativeunit-delete-members.md) |[directoryObject](directoryobject.md)| Remover um membro.|
|[Adicionar um scopedRoleMember](../api/administrativeunit-post-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Atribua uma Azure AD com escopo de unidade administrativa.|
|[Listar scopedRoleMembers](../api/administrativeunit-list-scopedrolemembers.md) |Coleção [scopedRoleMembership](scopedrolemembership.md)| Listar Azure AD atribuições de função com escopo de unidade administrativa.|
|[Obter um scopedRoleMember](../api/administrativeunit-get-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Obtenha uma atribuição Azure AD função com escopo de unidade administrativa.|
|[Remover um scopedRoleMember](../api/administrativeunit-delete-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Remova uma atribuição Azure AD função com escopo de unidade administrativa.|
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension-get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obtenha uma extensão aberta identificada pelo nome da extensão.|
|**Extensões de esquema**| | |
|[Adicionar valores de extensões de esquema](/graph/extensibility-schema-groups) || Cria uma definição para a extensão de esquema e usa-a para adicionar dados digitados personalizados a um recurso.|

> [!NOTE]
> O ponto de extremidade de URL para chamar a API `/administrativeUnits` **administrativeUnits** está no ponto `beta` de extremidade, mas `/directory/administrativeUnits` no ponto `v1.0` de extremidade.

## <a name="properties"></a>Propriedades

> [!IMPORTANT]
> O uso específico de `$filter` e o parâmetro de consulta `$search` é suportado somente quando se usa o cabeçalho **ConsistencyLevel** definido como `eventual` e `$count`. Para obter mais informações, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries#administrative-unit-properties).

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|description|String|Uma descrição opcional para a unidade administrativa. Dá `$filter` suporte a (`eq`, `ne`, `in`, `startsWith`), `$search`.|
|displayName|Cadeia de caracteres|Nome de exibição da unidade administrativa. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores), `$search`, e `$orderBy`.|
|id|String|Identificador exclusivo para a unidade administrativa. Somente leitura. Suporta `$filter` (`eq`).|
| membershipRule | String | Regra de associação dinâmica para a unidade administrativa. Para obter mais informações sobre as regras que você pode usar para unidades administrativas dinâmicas e grupos dinâmicos, consulte [Usando atributos para criar regras avançadas](https://azure.microsoft.com/documentation/articles/active-directory-accessmanagement-groups-with-advanced-rules/). |
| membershipRuleProcessingState | String | Usado para controlar se a regra de associação dinâmica é processada ativamente. Defina como `On` quando você deseja que a regra de associação dinâmica esteja ativa `Paused` e se você deseja parar de atualizar a associação dinamicamente. Se não estiver definido, o comportamento padrão será `Paused`. |
| membershipType | Cadeia de caracteres | Tipo de associação para a unidade administrativa. Pode ser `dynamic` ou `assigned`. Se não estiver definido, o comportamento padrão será `assigned`. |
| visibility | Cadeia de caracteres | Controla se a unidade administrativa e seus membros estão ocultos ou públicos. Pode ser definido como `HiddenMembership` ou `Public`. Se não estiver definido, o comportamento padrão será `Public`. Quando definido como `HiddenMembership`, somente os membros da unidade administrativa podem listar outros membros da unidade administrativa. |

> [!TIP]
> Extensões de diretório e dados associados são retornados por padrão, enquanto extensões de esquema e dados associados retornados somente em `$select`.

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|extensions|Coleção [extension](extension.md)|A coleção de extensões abertas definidas para esta unidade administrativa. Anulável.|
|members|Coleção [directoryObject](directoryobject.md)|Usuários e grupos que são membros desta unidade administrativa. Suporta o `$expand`.|
|scopedRoleMembers|Coleção [scopedRoleMembership](scopedrolemembership.md)| Membros de função com escopo desta unidade administrativa.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.administrativeUnit"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "visibility": "String",
  "membershipType": "String",
  "membershipRule": "String",
  "membershipRuleProcessingState": "String"
}

```


## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas](/graph/extensibility-open-users)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "administrativeUnit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


