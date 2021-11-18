---
title: Tipo de recurso directory (itens excluídos)
description: . Itens excluídos permanecerão disponíveis para restauração por até 30 dias. Após 30 dias, esses itens serão excluídos permanentemente.
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 36fbef413478ac31fa4cafbc3f30166d6e318919
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077632"
---
# <a name="directory-resource-type"></a>tipo de recurso de diretório

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um item excluído no diretório. Quando um item é excluído, ele é adicionado ao "contêiner" de itens excluídos. Itens excluídos permanecerão disponíveis para restauração por até 30 dias. Após 30 dias, esses itens serão excluídos permanentemente.

Atualmente, a funcionalidade de itens excluídos só tem suporte para os recursos [de](application.md)aplicativo, [grupo](group.md) [e](user.md) usuário.

Herda da [entidade](entity.md).

## <a name="methods"></a>Methods

| Método         | Tipo de retorno | Descrição |
|:---------------|:------------|:------------|
|[Obter item excluído](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) | Obtém as propriedades de um item excluído. |
|[Restaurar item excluído](../api/directory-deleteditems-restore.md) |[directoryObject](directoryobject.md)| Restaura um item recentemente excluído. |
|[Listar itens excluídos](../api/directory-deleteditems-list.md) |Coleção [directoryObject](directoryobject.md)| Obtém uma lista de itens recentemente excluídos. |
|[Excluir permanentemente um item](../api/directory-deleteditems-delete.md) | Nenhum | Exclui permanentemente um item. |
|[Listar itens excluídos pertencentes a um usuário](../api/directory-deleteditems-user-owned.md) | Coleção [directoryObject](directoryobject.md) | Lista itens de diretório pertencentes a um usuário. |

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres| Um identificador exclusivo do objeto; por exemplo, `12345678-9abc-def0-1234-56789abcde` . Chave. Não anulável. Somente leitura. Herdado da [entidade](entity.md).|

## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|administrativeUnits|[Coleção administrativeUnit](administrativeunit.md)| Contêiner conceitual para objetos de diretório de grupo e usuário.|
|attributeSets|[Coleção attributeSet](attributeset.md)| Grupo de definições de atributos de segurança personalizados relacionados.|
|customSecurityAttributeDefinitions|[Coleção customSecurityAttributeDefinition](customsecurityattributedefinition.md)|Esquema de atributos de segurança personalizados (pares de valores-chave).|
|deleteditems|Coleção [directoryObject](directoryobject.md)| Itens recentemente excluídos. Somente leitura. Anulável.|
|featureRolloutPolicies|[Coleção featureRolloutPolicy](featurerolloutpolicy.md)| Anulável.|
|federationConfigurations|Coleção [identityProviderBase](../resources/identityproviderbase.md) |Configure a federação de domínio com organizações cujo provedor de identidade (IdP) oferece suporte ao protocolo SAML ou WS-Fed.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
  "@odata.type": "#microsoft.graph.directory"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


