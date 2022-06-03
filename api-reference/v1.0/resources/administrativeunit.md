---
title: Tipo de recurso administrativeUnit
description: Uma unidade administrativa fornece um contêiner conceitual para objetos de diretório de usuário, grupo e dispositivo.
ms.localizationpriority: medium
author: DougKirschner
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: de7c9260c5682c12f2d61cbc336f22ecb7579d20
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2022
ms.locfileid: "65883975"
---
# <a name="administrativeunit-resource-type"></a>Tipo de recurso administrativeUnit

Namespace: microsoft.graph

Uma unidade administrativa fornece um contêiner conceitual para objetos de diretório de usuário, grupo e dispositivo. Usando unidades administrativas, um administrador da empresa agora pode delegar responsabilidades administrativas para gerenciar os usuários, grupos e dispositivos contidos dentro ou no escopo de uma unidade administrativa para um administrador regional ou departamento. Esse recurso é um tipo aberto que permite que outras propriedades sejam passadas.

Vejamos um exemplo. Imagine que a Contoso Corp é composta por duas divisões: uma Divisão da Costa Oeste e uma Divisão da Costa Leste. As funções de diretório na Contoso têm como escopo todo o locatário. Lee, um administrador da empresa Contoso, deseja delegar responsabilidades administrativas, mas defina-as como escopo para a Divisão da Costa Oeste ou para a divisão da Costa Leste.  Lee pode criar uma *unidade admistrativa* da Costa Oeste e colocar todos os usuários da Costa Oeste nessa unidade administrativa.  Da mesma forma, Lee pode criar uma *unidade administrativa da Costa Leste*.  Agora Lee, pode começar a delegar responsabilidades administrativas a outras  pessoas, mas com escopo para as novas unidades administrativas que ele criou. Lee coloca Jennifer em uma *função de* administrador de assistência **técnica com** escopo para a *unidade administrativa da Costa Oeste*.  Isso permite que Jennifer redefina a senha de qualquer usuário, mas somente se esses usuários estão na *unidade administrativa da Costa Oeste*.  Da mesma forma, Lee coloca Dave em uma função de administrador de *conta* de **usuário** com escopo para a *unidade administrativa da Costa Leste*.  Isso permite que Dave atualize usuários, atribua licenças e redefina a senha de qualquer usuário, mas somente se esses usuários estão na unidade administrativa *da Costa Leste*. Para obter uma visão geral em vídeo, consulte [Introdução às Unidades Administrativas do Azure Active Directory](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units).


Este tópico fornece descrições das propriedades declaradas e das propriedades de navegação expostas pela entidade administrativeUnit, bem como as operações e funções que podem ser chamadas no recurso administrativeUnits.


## <a name="methods"></a>Métodos

| Método   | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Criar](../api/directory-post-administrativeunits.md) | [administrativeUnit](administrativeunit.md) | Crie uma nova unidade administrativa.|
|[Lista](../api/directory-list-administrativeunits.md) | [coleção administrativeUnit](administrativeunit.md) |Listar propriedades de todas as administrativeUnits.|
|[Get](../api/administrativeunit-get.md) | [administrativeUnit](administrativeunit.md) |Ler propriedades e relações de um objeto administrativeUnit específico.|
|[Atualizar](../api/administrativeunit-update.md) | [administrativeUnit](administrativeunit.md)    |Atualize o objeto administrativeUnit. |
|[Excluir](../api/administrativeunit-delete.md) | Nenhum |Exclua o objeto administrativeUnit. |
|[Adicionar um membro](../api/administrativeunit-post-members.md) |[directoryObject](directoryobject.md)| Adicione um membro (usuário, grupo ou dispositivo).|
|[Listar membros](../api/administrativeunit-list-members.md) |Coleção [directoryObject](directoryobject.md)| Obtenha a lista de membros (usuário, grupo ou dispositivo).|
|[Obter um membro](../api/administrativeunit-get-members.md) |[directoryObject](directoryobject.md)| Obter um membro específico.|
|[Remover um membro](../api/administrativeunit-delete-members.md) |[directoryObject](directoryobject.md)| Remover um membro.|
|[Adicionar membro de função com escopo](../api/administrativeunit-post-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Adicione um membro de função com escopo.|
|[Listar membros de função com escopo](../api/administrativeunit-list-scopedrolemembers.md) |Coleção [scopedRoleMembership](scopedrolemembership.md)| Obter a lista de administradores de função com escopo.|
|[Obter um membro de função com escopo](../api/administrativeunit-get-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Obter um membro de função com escopo específico.|
|[Remover um membro de função com escopo](../api/administrativeunit-delete-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Remover um membro de função com escopo.|

## <a name="properties"></a>Propriedades

> [!IMPORTANT]
> O uso específico de `$filter` e o parâmetro de consulta `$search` é suportado somente quando se usa o cabeçalho **ConsistencyLevel** definido como `eventual` e `$count`. Para obter mais informações, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries#administrative-unit-properties).

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|description|String|Uma descrição opcional para a unidade administrativa. Dá `$filter` suporte a (`eq`, `ne`, `in`, `startsWith`), `$search`.|
|displayName|String|Nome de exibição da unidade administrativa. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores), `$search`, e `$orderBy`.|
|id|String|Identificador exclusivo para a unidade administrativa. Somente leitura. Suporta `$filter` (`eq`).|
|visibility|String|Controla se a unidade administrativa e seus membros estão ocultos ou públicos. Pode ser definido como `HiddenMembership`. Se não estiver definido (o valor é `null`), o comportamento padrão será público. Quando definido como `HiddenMembership`, somente os membros da unidade administrativa podem listar outros membros da unidade administrativa.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|extensions|Coleção [extension](extension.md)|A coleção de extensões abertas definidas para esta unidade administrativa. Anulável.|
|members|Coleção [directoryObject](directoryobject.md)|Usuários e grupos que são membros desta unidade administrativa. Suporta o `$expand`.|
|scopedRoleMembers|Coleção [scopedRoleMembership](scopedrolemembership.md)| Membros de função com escopo desta unidade administrativa. |

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
  "visibility": "String"
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
