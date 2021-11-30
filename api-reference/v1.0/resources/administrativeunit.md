---
title: Tipo de recurso administrativeUnit
description: Uma unidade administrativa fornece um contêiner conceitual para objetos de diretório usuário e grupo.
ms.localizationpriority: medium
author: DougKirschner
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: fee9c6254dd06611a01378c88b516f4e58575ade
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226537"
---
# <a name="administrativeunit-resource-type"></a>Tipo de recurso administrativeUnit

Namespace: microsoft.graph

Uma unidade administrativa fornece um contêiner conceitual para objetos de diretório usuário e grupo. Usando unidades administrativas, um administrador da empresa agora pode delegar responsabilidades administrativas para gerenciar os usuários e grupos contidos dentro ou com escopo para uma unidade administrativa para um administrador regional ou departamento. Esse recurso é um tipo aberto que permite que outras propriedades sejam passadas.

Vejamos um exemplo. Imagine que a Contoso Corp é feita de duas divisões : uma Divisão da Costa Oeste e uma Divisão da Costa Leste. As funções de diretório na Contoso têm escopo para todo o locatário. Lee, administrador da empresa Contoso, deseja delegar responsabilidades administrativas, mas as escopo para a Divisão da Costa Oeste ou para a divisão da Costa Leste.  Lee pode criar uma *unidade admistrativa* da Costa Oeste e colocar todos os usuários da Costa Oeste nessa unidade administrativa.  Da mesma forma, Lee pode criar uma unidade administrativa da Costa *Leste.*  Agora, Lee pode começar a delegar  responsabilidades administrativas a outras pessoas, mas com escopo para as novas unidades administrativas que ele criou. Lee coloca Jennifer em *uma função de administrador de helpdesk* **com** escopo para a unidade administrativa da *Costa Oeste.*  Isso permite que a Jennifer redefinir a senha de qualquer usuário, mas somente se esses usuários estão na unidade administrativa *da Costa Oeste.*  Da mesma forma, Lee coloca Dave em uma função *de* administrador de conta de usuário com escopo **para** a unidade administrativa da Costa *Leste.*  Isso permite que Dave atualize usuários, atribua licenças e redefinir a senha de qualquer usuário, mas somente se esses usuários estão na unidade administrativa da Costa *Leste.* Para uma visão geral de vídeo, consulte [Introdução Azure Active Directory Unidades Administrativas](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units).


Este tópico fornece descrições das propriedades declaradas e propriedades de navegação expostas pela entidade administrativeUnit, bem como as operações e funções que podem ser chamadas no recurso administrativeUnits.


## <a name="methods"></a>Methods

| Método   | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Criar](../api/administrativeunit-post-administrativeunits.md) | [administrativeUnit](administrativeunit.md) | Crie uma nova unidade administrativa.|
|[List](../api/administrativeunit-list.md) | [Coleção administrativeUnit](administrativeunit.md) |Listar propriedades de todas as administrativeUnits.|
|[Get](../api/administrativeunit-get.md) | [administrativeUnit](administrativeunit.md) |Ler propriedades e relações de um objeto administrativeUnit específico.|
|[Atualizar](../api/administrativeunit-update.md) | [administrativeUnit](administrativeunit.md)    |Atualizar o objeto administrativeUnit. |
|[Excluir](../api/administrativeunit-delete.md) | Nenhum |Excluir objeto administrativeUnit. |
|[Adicionar um membro](../api/administrativeunit-post-members.md) |[directoryObject](directoryobject.md)| Adicionar um membro (usuário ou grupo).|
|[Listar membros](../api/administrativeunit-list-members.md) |Coleção [directoryObject](directoryobject.md)| Obter a lista de membros (usuário e grupo).|
|[Obter um membro](../api/administrativeunit-get-members.md) |[directoryObject](directoryobject.md)| Obter um membro específico.|
|[Remover um membro](../api/administrativeunit-delete-members.md) |[directoryObject](directoryobject.md)| Remova um membro.|
|[Adicionar membro de função com escopo](../api/administrativeunit-post-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Adicione um membro de função com escopo.|
|[Listar membros de função com escopo](../api/administrativeunit-list-scopedrolemembers.md) |Coleção [scopedRoleMembership](scopedrolemembership.md)| Obter a lista de administradores de função de escopo.|
|[Obter um membro de função com escopo](../api/administrativeunit-get-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Obter um membro de função de escopo específico.|
|[Remover um membro de função com escopo](../api/administrativeunit-delete-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Remova um membro de função com escopo.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|description|string|Uma descrição opcional para a unidade administrativa.|
|displayName|string|Nome de exibição da unidade administrativa.|
|id|string|Identificador exclusivo da unidade administrativa. Apenas leitura.|
|visibilidade|string|Controla se a unidade administrativa e seus membros estão ocultos ou públicos. Pode ser definido como `HiddenMembership` ou `Public` . Se não estiver definido, o comportamento padrão será `Public` . Quando definido como `HiddenMembership` , somente membros da unidade administrativa podem listar outros membros da unidade administrativa.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|extensions|Coleção [extension](extension.md)|A coleção de extensões abertas definidas para esta Unidade Administrativa. Anulável.|
|members|Coleção [directoryObject](directoryobject.md)|Usuários e grupos que são membros desta Unidade Adminsitrative. Métodos HTTP: GET (membros da lista), POST (adicionar membros), DELETE (remover membros).|
|scopedRoleMembers|Coleção [scopedRoleMembership](scopedrolemembership.md)| Membros de função de escopo desta Unidade Administrativa.  Métodos HTTP: GET (list scopedRoleMemberships), POST (adicionar scopedRoleMembership), DELETE (remover scopedRoleMembership). |

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
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "visibility": "string"
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
