---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
description: O recurso UploadSession fornece informações sobre como carregar arquivos grandes no OneDrive, no OneDrive for Business ou em bibliotecas de documentos do SharePoint, ou como anexos de arquivo para objetos de eventos e mensagens do Outlook.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ff7ed4278da4d04d1af5158ce8fc01011bcc8598
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090610"
---
# <a name="uploadsession-resource-type"></a><span data-ttu-id="e1dab-103">tipo de recurso uploadSession</span><span class="sxs-lookup"><span data-stu-id="e1dab-103">uploadSession resource type</span></span>

<span data-ttu-id="e1dab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1dab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e1dab-105">O recurso **uploadSession** fornece informações sobre como carregar arquivos grandes no onedrive, no onedrive for Business ou em bibliotecas de documentos do SharePoint ou em [eventos de evento](event.md) e de [mensagem](message.md) do Outlook como anexos.</span><span class="sxs-lookup"><span data-stu-id="e1dab-105">The **uploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries, or to Outlook [event](event.md) and [message](message.md) items as attachments.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1dab-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1dab-106">JSON representation</span></span>

<span data-ttu-id="e1dab-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e1dab-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="e1dab-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1dab-108">Properties</span></span>


| <span data-ttu-id="e1dab-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1dab-109">Property</span></span>       | <span data-ttu-id="e1dab-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1dab-110">Type</span></span>              |<span data-ttu-id="e1dab-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1dab-111">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="e1dab-112">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e1dab-112">expirationDateTime</span></span> | <span data-ttu-id="e1dab-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1dab-113">DateTimeOffset</span></span>    | <span data-ttu-id="e1dab-p101">Data e hora em UTC em que a sessão de carregamento expirará. O arquivo completo deve ser carregado antes que esta hora de expiração seja atingida.</span><span class="sxs-lookup"><span data-stu-id="e1dab-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="e1dab-116">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="e1dab-116">nextExpectedRanges</span></span> | <span data-ttu-id="e1dab-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1dab-117">String collection</span></span> | <span data-ttu-id="e1dab-118">Uma coleção de intervalos de bytes que estão ausentes do servidor para o arquivo.</span><span class="sxs-lookup"><span data-stu-id="e1dab-118">A collection of byte ranges that the server is missing for the file.</span></span> <span data-ttu-id="e1dab-119">Estes intervalos são indexados como zero e têm o formato "início-fim" (por exemplo "0-26" para indicar os primeiros 27 bytes do arquivo).</span><span class="sxs-lookup"><span data-stu-id="e1dab-119">These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span> <span data-ttu-id="e1dab-120">Ao carregar arquivos como anexos do Outlook, em vez de uma coleção de intervalos, essa propriedade sempre indica um valor único "{Start}", o local no arquivo em que o próximo carregamento deve começar.</span><span class="sxs-lookup"><span data-stu-id="e1dab-120">When uploading files as Outlook attachments, instead of a collection of ranges, this property always indicates a single value "{start}", the location in the file where the next upload should begin.</span></span>
| <span data-ttu-id="e1dab-121">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="e1dab-121">uploadUrl</span></span>          | <span data-ttu-id="e1dab-122">String</span><span class="sxs-lookup"><span data-stu-id="e1dab-122">String</span></span>            | <span data-ttu-id="e1dab-123">O ponto de extremidade de URL que aceita solicitações PUT para intervalos de bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="e1dab-123">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="e1dab-124">Confira também</span><span class="sxs-lookup"><span data-stu-id="e1dab-124">See also</span></span>

- [<span data-ttu-id="e1dab-125">Anexar arquivos grandes a mensagens e eventos do Outlook como anexos </span><span class="sxs-lookup"><span data-stu-id="e1dab-125">Attach large files to Outlook messages and events as attachments </span></span>](/graph/outlook-large-attachments)
- [<span data-ttu-id="e1dab-126">Carregar arquivos grandes com uma sessão de upload</span><span class="sxs-lookup"><span data-stu-id="e1dab-126">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->

