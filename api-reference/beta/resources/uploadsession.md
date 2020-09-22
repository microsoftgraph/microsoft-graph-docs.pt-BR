---
author: JeremyKelley
description: Representa informações de um processo interativo para carregar arquivos grandes para o OneDrive, o OneDrive for Business ou as bibliotecas de documentos do SharePoint, ou como anexos de arquivo para objetos de eventos e mensagens do Outlook.
title: tipo de recurso uploadSession
localization_priority: Normal
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 9dd76265e08cc377aba295679a35f33f2256b3b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003441"
---
# <a name="uploadsession-resource-type"></a><span data-ttu-id="21801-103">tipo de recurso uploadSession</span><span class="sxs-lookup"><span data-stu-id="21801-103">uploadSession resource type</span></span>

<span data-ttu-id="21801-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21801-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21801-105">Representa informações de um processo interativo para carregar arquivos grandes para o OneDrive, o OneDrive for Business ou as bibliotecas de documentos do SharePoint ou para [eventos de evento](event.md) e de [mensagem](message.md) do Outlook como anexos.</span><span class="sxs-lookup"><span data-stu-id="21801-105">Represents information for an iterative process to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries, or to Outlook [event](event.md) and [message](message.md) items as attachments.</span></span>

## <a name="json-representation"></a><span data-ttu-id="21801-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21801-106">JSON representation</span></span>

<span data-ttu-id="21801-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="21801-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "uploadUrl", "nextExpectedRanges" ],
  "@odata.type": "microsoft.graph.uploadSession",
  "baseType": null
}-->

```json
{
  "uploadUrl": "String",
  "expirationDateTime": "String (timestamp)",
  "nextExpectedRanges": ["String"]
}
```

## <a name="properties"></a><span data-ttu-id="21801-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21801-108">Properties</span></span>


| <span data-ttu-id="21801-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21801-109">Property</span></span>       | <span data-ttu-id="21801-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="21801-110">Type</span></span>              |<span data-ttu-id="21801-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="21801-111">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="21801-112">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="21801-112">expirationDateTime</span></span> | <span data-ttu-id="21801-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21801-113">DateTimeOffset</span></span>    | <span data-ttu-id="21801-p101">Data e hora em UTC em que a sessão de carregamento expirará. O arquivo completo deve ser carregado antes que esta hora de expiração seja atingida.</span><span class="sxs-lookup"><span data-stu-id="21801-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="21801-116">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="21801-116">nextExpectedRanges</span></span> | <span data-ttu-id="21801-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="21801-117">String collection</span></span> | <span data-ttu-id="21801-118">Ao carregar arquivos em bibliotecas de documentos, esta é uma coleção de intervalos de bytes que o servidor está faltando para o arquivo.</span><span class="sxs-lookup"><span data-stu-id="21801-118">When uploading files to document libraries, this is a collection of byte ranges that the server is missing for the file.</span></span> <span data-ttu-id="21801-119">Esses intervalos são indexados por zero e do formato, "{Start}-{End}" (por exemplo, "0-26" para indicar os primeiros 27 bytes do arquivo).</span><span class="sxs-lookup"><span data-stu-id="21801-119">These ranges are zero-indexed and of the format, "{start}-{end}" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span> <span data-ttu-id="21801-120">Ao carregar arquivos como anexos do Outlook, em vez de uma coleção de intervalos, essa propriedade sempre indica um valor único "{Start}", o local no arquivo em que o próximo carregamento deve começar.</span><span class="sxs-lookup"><span data-stu-id="21801-120">When uploading files as Outlook attachments, instead of a collection of ranges, this property always indicates a single value "{start}", the location in the file where the next upload should begin.</span></span>
| <span data-ttu-id="21801-121">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="21801-121">uploadUrl</span></span>          | <span data-ttu-id="21801-122">String</span><span class="sxs-lookup"><span data-stu-id="21801-122">String</span></span>            | <span data-ttu-id="21801-123">O ponto de extremidade de URL que aceita solicitações PUT para intervalos de bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="21801-123">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="21801-124">Confira também</span><span class="sxs-lookup"><span data-stu-id="21801-124">See also</span></span>

- [<span data-ttu-id="21801-125">Anexar arquivos grandes a mensagens e eventos do Outlook como anexos </span><span class="sxs-lookup"><span data-stu-id="21801-125">Attach large files to Outlook messages and events as attachments </span></span>](/graph/outlook-large-attachments)
- [<span data-ttu-id="21801-126">Carregar arquivos grandes com uma sessão de upload</span><span class="sxs-lookup"><span data-stu-id="21801-126">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession",
  "suppressions": []
}
-->


