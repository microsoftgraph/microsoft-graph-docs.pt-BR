---
title: tipo de recurso de educationFileResource
description: Uma subclasse de educationResource que representa um objeto de arquivo que está associado a atribuição ou o envio.  Nesse caso, o arquivo não é um dos arquivos especiais (Word, Excel e assim por diante), mas é um arquivo que não tem manipulação especial dentro do sistema. O recurso de arquivo deve ser armazenado em **resourceFolder** que está associado a atribuição ou o envio que este recurso está anexado.
ms.openlocfilehash: b3ba77b6b9243d987ad1137afe6d2206e47dadaf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037215"
---
# <a name="educationfileresource-resource-type"></a><span data-ttu-id="947db-105">tipo de recurso de educationFileResource</span><span class="sxs-lookup"><span data-stu-id="947db-105">educationFileResource resource type</span></span>

> <span data-ttu-id="947db-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="947db-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="947db-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="947db-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="947db-108">Uma subclasse de [educationResource](educationresource.md) que representa um objeto de arquivo que está associado a atribuição ou o envio.</span><span class="sxs-lookup"><span data-stu-id="947db-108">A subclass of [educationResource](educationresource.md) that represents a file object that is associated with the assignment or submission.</span></span>  <span data-ttu-id="947db-109">Nesse caso, o arquivo não é um dos arquivos especiais (Word, Excel e assim por diante), mas é um arquivo que não tem manipulação especial dentro do sistema.</span><span class="sxs-lookup"><span data-stu-id="947db-109">In this case, the file is not one of the special files (Word, Excel, and so on) but is a file that does not have special handling within the system.</span></span> <span data-ttu-id="947db-110">O recurso de arquivo deve ser armazenado em **resourceFolder** que está associado a atribuição ou o envio que este recurso está anexado.</span><span class="sxs-lookup"><span data-stu-id="947db-110">The file resource must be stored in the **resourceFolder** that is associated with the assignment or submission this resource is attached to.</span></span>

## <a name="properties"></a><span data-ttu-id="947db-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="947db-111">Properties</span></span>
| <span data-ttu-id="947db-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="947db-112">Property</span></span>     | <span data-ttu-id="947db-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="947db-113">Type</span></span>   |<span data-ttu-id="947db-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="947db-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="947db-115">fileUrl</span><span class="sxs-lookup"><span data-stu-id="947db-115">fileUrl</span></span>|<span data-ttu-id="947db-116">String</span><span class="sxs-lookup"><span data-stu-id="947db-116">String</span></span>|<span data-ttu-id="947db-117">Local no disco do recurso de arquivo.</span><span class="sxs-lookup"><span data-stu-id="947db-117">Location on disk of the file resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="947db-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="947db-118">JSON representation</span></span>

<span data-ttu-id="947db-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="947db-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->