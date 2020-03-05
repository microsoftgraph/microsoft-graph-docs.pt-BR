---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
description: O recurso UploadSession fornece informações sobre como carregar arquivos grandes no OneDrive, no OneDrive for Business ou em bibliotecas de documentos do SharePoint.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3537a59da65499e67283d8a0640e5392c65edce1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446783"
---
# <a name="uploadsession-resource"></a><span data-ttu-id="b258f-103">Recurso UploadSession</span><span class="sxs-lookup"><span data-stu-id="b258f-103">UploadSession resource</span></span>

<span data-ttu-id="b258f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b258f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b258f-105">O recurso **UploadSession** fornece informações sobre como carregar arquivos grandes no OneDrive, no OneDrive for Business ou em bibliotecas de documentos do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b258f-105">The **UploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b258f-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b258f-106">JSON representation</span></span>

<span data-ttu-id="b258f-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b258f-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "uploadUrl", "nextExpectedRanges" ],
  "@odata.type": "microsoft.graph.uploadSession"
}-->

```json
{
  "uploadUrl": "https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337",
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["0-"]
}
```

## <a name="properties"></a><span data-ttu-id="b258f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b258f-108">Properties</span></span>


| <span data-ttu-id="b258f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b258f-109">Property</span></span>       | <span data-ttu-id="b258f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b258f-110">Type</span></span>              |<span data-ttu-id="b258f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b258f-111">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="b258f-112">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b258f-112">expirationDateTime</span></span> | <span data-ttu-id="b258f-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b258f-113">DateTimeOffset</span></span>    | <span data-ttu-id="b258f-p101">Data e hora em UTC em que a sessão de carregamento expirará. O arquivo completo deve ser carregado antes que esta hora de expiração seja atingida.</span><span class="sxs-lookup"><span data-stu-id="b258f-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="b258f-116">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="b258f-116">nextExpectedRanges</span></span> | <span data-ttu-id="b258f-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b258f-117">String collection</span></span> | <span data-ttu-id="b258f-p102">Uma coleção de intervalos de bytes que estão ausentes do servidor para o arquivo. Estes intervalos são indexados como zero e têm o formato "início-fim" (por exemplo "0-26" para indicar os primeiros 27 bytes do arquivo).</span><span class="sxs-lookup"><span data-stu-id="b258f-p102">A collection of byte ranges that the server is missing for the file. These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span>
| <span data-ttu-id="b258f-120">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="b258f-120">uploadUrl</span></span>          | <span data-ttu-id="b258f-121">String</span><span class="sxs-lookup"><span data-stu-id="b258f-121">String</span></span>            | <span data-ttu-id="b258f-122">O ponto de extremidade de URL que aceita solicitações PUT para intervalos de bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="b258f-122">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="b258f-123">Confira também</span><span class="sxs-lookup"><span data-stu-id="b258f-123">See also</span></span>

- [<span data-ttu-id="b258f-124">Carregar arquivos grandes com uma sessão de upload</span><span class="sxs-lookup"><span data-stu-id="b258f-124">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->
