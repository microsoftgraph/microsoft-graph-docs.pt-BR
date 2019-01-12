---
title: tipo de recurso de administrativeUnit
description: Uma unidade administrativa fornece um contêiner conceitual para objetos de diretório de usuário e grupo. Usando unidades administrativas, um administrador da empresa agora pode delegar responsabilidades administrativas para gerenciar os usuários e grupos contidos dentro ou com escopo para uma unidade administrativa a um administrador departamental ou regional.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a4fb81c9a9d605dd155facefb263ff4a310442c3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955314"
---
# <a name="administrativeunit-resource-type"></a>tipo de recurso de administrativeUnit

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Uma unidade administrativa fornece um contêiner conceitual para objetos de diretório de usuário e grupo. Usando unidades administrativas, um administrador da empresa agora pode delegar responsabilidades administrativas para gerenciar os usuários e grupos contidos dentro ou com escopo para uma unidade administrativa a um administrador departamental ou regional.

Vamos ver um exemplo. Imagine que Contoso Corp é composta por duas divisões - uma divisão Costa Oeste e uma divisão Costa Leste. Funções de diretório na Contoso têm o escopo para o inquilino inteiro. Lee, um administrador da empresa Contoso, deseja delegar responsabilidades administrativas, mas o escopo-los a divisão da Costa Oeste ou a divisão da Costa Leste.  Lee pode criar uma *unidade de admistrative Costa Oeste* e coloque todos os usuários da Costa Oeste nesta unidade administrativa.  Da mesma forma, Lee pode criar uma *unidade de administrativas Costa Leste*.  Agora Lee, pode iniciar delegando responsabilidades administrativas para outras pessoas, mas **com escopo** para as novas unidades administrativas que ele é criado. Lee coloca Jennifer em um *administrador de assistência técnica* função **com escopo** para a *unidade administrativa da Costa Oeste*.  Isso permite Jennifer redefinir qualquer senha de usuário, mas somente se os usuários estiverem na *unidade administrativa da Costa Oeste*.  Da mesma forma, Lee coloca Dave em um *administrador da conta de usuário* função **com escopo** para a *unidade administrativa da Costa Leste*.  Isso permite Dave atualizar usuários, atribuir licenças e redefinir a senha do usuário, qualquer, mas somente se os usuários estão na *unidade administrativa da Costa Leste*. Para obter uma visão de vídeo, consulte [Introdução à unidades administrativas do Azure Active Directory](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units).

Esse recurso permite que você adicione seus próprios dados às propriedades personalizadas usando [extensions](/graph/extensibility-overview).

Este tópico fornece descrições das propriedades declaradas e propriedades de navegação expostas da entidade administrativeUnit, bem como as operações e funções que podem ser chamadas no recurso administrativeUnits.


## <a name="methods"></a>Métodos

| Método   | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Criar administrativeUnit](../api/administrativeunit-post-administrativeunits.md) | [administrativeUnit](administrativeunit.md) | Crie uma nova unidade administrativa.|
|[Lista administrativeUnits](../api/administrativeunit-list.md) | coleção [administrativeUnit](administrativeunit.md) |Propriedades de lista de todos os administrativeUnits.|
|[Obter administrativeUnit](../api/administrativeunit-get.md) | [administrativeUnit](administrativeunit.md) |Leia as propriedades e os relacionamentos de um objeto administrativeUnit específico.|
|[Atualizar adminstrativeUnit](../api/administrativeunit-update.md) | [administrativeUnit](administrativeunit.md)  |Atualize o objeto administrativeUnit. |
|[Excluir adminstrativeUnit](../api/administrativeunit-delete.md) | Nenhum |Exclua objeto administrativeUnit. |
|[Adicionar um membro](../api/administrativeunit-post-members.md) |[directoryObject](directoryobject.md)| Adicione um participante (usuário ou grupo).|
|[Listar membros](../api/administrativeunit-list-members.md) |Coleção [directoryObject](directoryobject.md)| Obtenha a lista de membros (de usuário e de grupo).|
|[Obter membro](../api/administrativeunit-get-members.md) |[directoryObject](directoryobject.md)| Obtenha um determinado membro.|
|[Remover um membro](../api/administrativeunit-delete-members.md) |[directoryObject](directoryobject.md)| Remova um membro.|
|[Adicionar um membro da função com escopo](../api/administrativeunit-post-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Adicione um membro da função com escopo.|
|[Membros da função com escopo de lista](../api/administrativeunit-list-scopedrolemembers.md) |coleção [scopedRoleMembership](scopedrolemembership.md)| Obter a lista de administradores de função com escopo.|
|[Obtenha um membro da função com escopo](../api/administrativeunit-get-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Obtenha um determinado membro da função com escopo.|
|[Remover um membro da função com escopo](../api/administrativeunit-delete-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Remova um membro da função com escopo.|
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension-get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obtenha uma extensão aberta identificada pelo nome da extensão.|
|**Extensões de esquema**| | |
|[Adicionar valores de extensões de esquema](/graph/extensibility-schema-groups) || Criar uma definição para a extensão de esquema e usá-la para adicionar dados digitados personalizados a um recurso.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|description|string|Uma descrição opcional para a unidade administrativa.|
|displayName|string|Nome de exibição para a unidade administrativa.|
|id|string|Identificador exclusivo para a unidade administrativa. Somente leitura.|
|visibilidade|string|Controla se a unidade administrativos e seus membros estão ocultos ou público. Pode ser definido como HiddenMembership ou público. Se não for definido, o comportamento padrão é público. Quando definido como HiddenMembership, somente os membros da unidade administrativa podem listar outros membros da unidade administrativas.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|extensions|Coleção [extension](extension.md)|A coleção de extensões open definidos para esta unidade administrativa. Anulável.|
|membros|Coleção [directoryObject](directoryobject.md)|Usuários e grupos que são membros desta unidade Adminsitrative. Métodos HTTP: Obtenha (membros de lista), POST (adicionar membros), DELETE (remover membros).|
|scopedRoleMembers|coleção [scopedRoleMembership](scopedrolemembership.md)| Membros da função com escopo desta unidade administrativa.  Métodos HTTP: Obtenha (scopedRoleMemberships lista), POST (Adicionar scopedRoleMembership), DELETE (remove scopedRoleMembership). |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
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
<!-- {
  "type": "#page.annotation",
  "description": "administrativeUnit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
