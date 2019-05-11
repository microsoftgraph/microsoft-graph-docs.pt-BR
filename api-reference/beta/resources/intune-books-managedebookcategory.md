---
title: tipo de recurso managedEBookCategory
description: Contém propriedades de uma única categoria de eBook do Intune.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0baa3dbbecd90483eeb182edf486fcd6bfdd846b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949315"
---
# <a name="managedebookcategory-resource-type"></a>tipo de recurso managedEBookCategory

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades de uma única categoria de eBook do Intune.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedEBookCategories](../api/intune-books-managedebookcategory-list.md)|coleção [managedEBookCategory](../resources/intune-books-managedebookcategory.md)|Listar Propriedades e relações dos objetos [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .|
|[Obter managedEBookCategory](../api/intune-books-managedebookcategory-get.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|Leia as propriedades e as relações do objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .|
|[Criar managedEBookCategory](../api/intune-books-managedebookcategory-create.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|Criar um novo objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .|
|[Excluir managedEBookCategory](../api/intune-books-managedebookcategory-delete.md)|Nenhum|Exclui [managedEBookCategory](../resources/intune-books-managedebookcategory.md).|
|[Atualizar managedEBookCategory](../api/intune-books-managedebookcategory-update.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|Atualiza as propriedades de um objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A chave da entidade.|
|displayName|String|O nome da categoria eBook.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o ManagedEBookCategory foi modificado pela última vez.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```




