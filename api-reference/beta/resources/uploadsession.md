---
author: JeremyKelley
description: Representa informações de um processo interativo para carregar arquivos grandes para o OneDrive, o OneDrive for Business ou bibliotecas de documentos do SharePoint, ou como anexos de arquivo para objetos de mensagem do Outlook.
title: tipo de recurso uploadSession
localization_priority: Normal
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 43086486175add54a7fe809eb9dffb8b3747c92a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519572"
---
# <a name="uploadsession-resource-type"></a><span data-ttu-id="11aaa-103">tipo de recurso uploadSession</span><span class="sxs-lookup"><span data-stu-id="11aaa-103">uploadSession resource type</span></span>

<span data-ttu-id="11aaa-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="11aaa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11aaa-105">Representa informações de um processo interativo para carregar arquivos grandes para o OneDrive, o OneDrive for Business ou bibliotecas de documentos do SharePoint, ou para objetos de [mensagem](message.md) do Outlook como anexos.</span><span class="sxs-lookup"><span data-stu-id="11aaa-105">Represents information for an iterative process to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries, or to Outlook [message](message.md) objects as attachments.</span></span>

## <a name="json-representation"></a><span data-ttu-id="11aaa-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11aaa-106">JSON representation</span></span>

<span data-ttu-id="11aaa-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="11aaa-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="11aaa-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11aaa-108">Properties</span></span>


| <span data-ttu-id="11aaa-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11aaa-109">Property</span></span>       | <span data-ttu-id="11aaa-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="11aaa-110">Type</span></span>              |<span data-ttu-id="11aaa-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="11aaa-111">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="11aaa-112">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="11aaa-112">expirationDateTime</span></span> | <span data-ttu-id="11aaa-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11aaa-113">DateTimeOffset</span></span>    | <span data-ttu-id="11aaa-p101">Data e hora em UTC em que a sessão de carregamento expirará. O arquivo completo deve ser carregado antes que esta hora de expiração seja atingida.</span><span class="sxs-lookup"><span data-stu-id="11aaa-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="11aaa-116">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="11aaa-116">nextExpectedRanges</span></span> | <span data-ttu-id="11aaa-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="11aaa-117">String collection</span></span> | <span data-ttu-id="11aaa-118">Ao carregar arquivos em bibliotecas de documentos, esta é uma coleção de intervalos de bytes que o servidor está faltando para o arquivo.</span><span class="sxs-lookup"><span data-stu-id="11aaa-118">When uploading files to document libraries, this is a collection of byte ranges that the server is missing for the file.</span></span> <span data-ttu-id="11aaa-119">Esses intervalos são indexados por zero e do formato, "{Start}-{End}" (por exemplo, "0-26" para indicar os primeiros 27 bytes do arquivo).</span><span class="sxs-lookup"><span data-stu-id="11aaa-119">These ranges are zero-indexed and of the format, "{start}-{end}" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span> <span data-ttu-id="11aaa-120">Ao carregar arquivos como anexos de mensagem do Outlook, em vez de uma coleção de intervalos, essa propriedade sempre indica um valor único "{Start}", o local no arquivo em que o próximo carregamento deve começar.</span><span class="sxs-lookup"><span data-stu-id="11aaa-120">When uploading files as Outlook message attachments, instead of a collection of ranges, this property always indicates a single value "{start}", the location in the file where the next upload should begin.</span></span>
| <span data-ttu-id="11aaa-121">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="11aaa-121">uploadUrl</span></span>          | <span data-ttu-id="11aaa-122">String</span><span class="sxs-lookup"><span data-stu-id="11aaa-122">String</span></span>            | <span data-ttu-id="11aaa-123">O ponto de extremidade de URL que aceita solicitações PUT para intervalos de bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="11aaa-123">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="11aaa-124">Confira também</span><span class="sxs-lookup"><span data-stu-id="11aaa-124">See also</span></span>

- [<span data-ttu-id="11aaa-125">Anexar arquivos grandes às mensagens do Outlook como anexos</span><span class="sxs-lookup"><span data-stu-id="11aaa-125">Attach large files to Outlook messages as attachments </span></span>](/graph/outlook-large-attachments)
- [<span data-ttu-id="11aaa-126">Carregar arquivos grandes com uma sessão de upload</span><span class="sxs-lookup"><span data-stu-id="11aaa-126">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

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
