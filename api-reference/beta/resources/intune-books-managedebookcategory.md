---
title: Tipo de recurso managedEBookCategory
description: Contém propriedades para uma única categoria de eBook do Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6b228c410565fe18d9f3b124e7fc176380d9c2b6
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58794860"
---
# <a name="managedebookcategory-resource-type"></a>Tipo de recurso managedEBookCategory

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém propriedades para uma única categoria de eBook do Intune.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedEBookCategories](../api/intune-books-managedebookcategory-list.md)|[Coleção managedEBookCategory](../resources/intune-books-managedebookcategory.md)|Listar propriedades e relações dos [objetos managedEBookCategory.](../resources/intune-books-managedebookcategory.md)|
|[Obter managedEBookCategory](../api/intune-books-managedebookcategory-get.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|Leia propriedades e relações do [objeto managedEBookCategory.](../resources/intune-books-managedebookcategory.md)|
|[Criar managedEBookCategory](../api/intune-books-managedebookcategory-create.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|Crie um novo [objeto managedEBookCategory.](../resources/intune-books-managedebookcategory.md)|
|[Excluir managedEBookCategory](../api/intune-books-managedebookcategory-delete.md)|Nenhum(a)|Exclui [managedEBookCategory](../resources/intune-books-managedebookcategory.md).|
|[Atualizar managedEBookCategory](../api/intune-books-managedebookcategory-update.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|Atualize as propriedades de [um objeto managedEBookCategory.](../resources/intune-books-managedebookcategory.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A chave da entidade.|
|displayName|Cadeia de caracteres|O nome da categoria de eBook.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que ManagedEBookCategory foi modificada pela última vez.|

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



