---
author: JeremyKelley
ms.date: 09/10/2017
title: SpecialFolder
localization_priority: Normal
description: O recurso SpecialFolder agrupa itens de dados relacionados a pastas especiais em uma única estrutura.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 696333867f06295640574449780db3f239674aedcbea3ce81c283c6f84211704
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180443"
---
# <a name="specialfolder-resource-type"></a>Tipo de recurso SpecialFolder

Namespace: microsoft.graph

O recurso **SpecialFolder** agrupa itens de dados relacionados a pastas especiais em uma única estrutura.

Se um **DriveItem** tiver uma faceta **specialFolder** não nula, o item representará uma pasta especial (nomeada).
Pastas especiais que podem ser acessadas diretamente por meio da [coleção de pastas especiais](../api/drive-get-specialfolder.md).

Pastas especiais fornecem aliases simples para acessar pastas conhecidas sem a necessidade de pesquisar a pasta pelo caminho (o que exigiria a localização) ou fazer referência à pasta com uma ID. Se uma pasta especial for renomeada ou movida para outro local na unidade de disco, esta sintaxe continuará a retornar a pasta.

As pastas especiais são criadas automaticamente na primeira vez que um aplicativo tenta gravar em uma, caso ainda não existam. Se um usuário excluir uma, ela será recriada quando algo for gravado nela novamente.

**Observação:** Se seu aplicativo solicitou apenas o escopo **Files.Read** e solicitar uma pasta especial que não exista, a resposta será um erro `403 Forbidden`.

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.specialFolder"
}-->
```json
{
  "name": "string"
}
```

## <a name="properties"></a>Propriedades

| Propriedade  | Tipo   | Descrição                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| nome      | string | O identificador exclusivo deste item na coleção `/drive/special` |

## <a name="special-folders"></a>Pastas especiais

Aqui estão as pastas especiais disponíveis no OneDrive Personal e no OneDrive for Business.

| Nome        | Id da pasta    | Descrição                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| Raiz de Aplicativo    | `approot`    | Pasta pessoal do aplicativo. Geralmente em `/Apps/{Application Name}` |
| Imagens da Câmera | `cameraroll` | A pasta de Backup de Imagens da Câmera. Não disponível no OneDrive for Business.   |
| Documentos   | `documents`  | A pasta Documentos.                                                    |
| Música       | `music`      | Pasta Música. Não disponível no OneDrive for Business.                |
| Fotos      | `photos`     | A pasta Fotos.                                                       |

## <a name="remarks"></a>Comentários 

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The SpecialFolder facet provides information about folders accessible as special folders.",
  "keywords": "special folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SpecialFolder"
} -->

