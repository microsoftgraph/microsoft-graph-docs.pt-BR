---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: UploadSession
ms.openlocfilehash: d84b588c28791ab8f1cf6cef1be6af767fa18e47
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="uploadsession-resource"></a><span data-ttu-id="f2d36-102">Recurso UploadSession</span><span class="sxs-lookup"><span data-stu-id="f2d36-102">UploadSession resource</span></span>

<span data-ttu-id="f2d36-103">O recurso **UploadSession** fornece informações sobre como carregar arquivos grandes no OneDrive, no OneDrive for Business ou em bibliotecas de documentos do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f2d36-103">The **UploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2d36-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2d36-104">JSON representation</span></span>

<span data-ttu-id="f2d36-105">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f2d36-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="f2d36-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2d36-106">Properties</span></span>


| <span data-ttu-id="f2d36-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2d36-107">Property</span></span>       | <span data-ttu-id="f2d36-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2d36-108">Type</span></span>              |<span data-ttu-id="f2d36-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2d36-109">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="f2d36-110">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f2d36-110">expirationDateTime</span></span> | <span data-ttu-id="f2d36-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2d36-111">DateTimeOffset</span></span>    | <span data-ttu-id="f2d36-p101">Data e hora em UTC em que a sessão de carregamento expirará. O arquivo completo deve ser carregado antes que esta hora de expiração seja atingida.</span><span class="sxs-lookup"><span data-stu-id="f2d36-p101">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="f2d36-114">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="f2d36-114">nextExpectedRanges</span></span> | <span data-ttu-id="f2d36-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2d36-115">String collection</span></span> | <span data-ttu-id="f2d36-p102">Uma coleção de intervalos de bytes que estão ausentes do servidor para o arquivo. Estes intervalos são indexados como zero e têm o formato "início-fim" (por exemplo "0-26" para indicar os primeiros 27 bytes do arquivo).</span><span class="sxs-lookup"><span data-stu-id="f2d36-p102">A collection of byte ranges that the server is missing for the file. These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span>
| <span data-ttu-id="f2d36-118">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="f2d36-118">uploadUrl</span></span>          | <span data-ttu-id="f2d36-119">String</span><span class="sxs-lookup"><span data-stu-id="f2d36-119">String</span></span>            | <span data-ttu-id="f2d36-120">O ponto de extremidade de URL que aceita solicitações PUT para intervalos de bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="f2d36-120">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="f2d36-121">Recursos adicionais</span><span class="sxs-lookup"><span data-stu-id="f2d36-121">Additional Resources</span></span>

<span data-ttu-id="f2d36-122">Confira [Carregar arquivos grandes com uma sessão de carregamento](../api/driveitem_createuploadsession.md) para saber mais sobre como carregar arquivos usando uma sessão de carregamento.</span><span class="sxs-lookup"><span data-stu-id="f2d36-122">See [Upload large files with an upload session](../api/driveitem_createuploadsession.md) for details on how to upload files using an upload session.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->
