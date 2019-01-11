---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
ms.openlocfilehash: 928dc79ae62b5b8b6f6789e42c719eb832135dcb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847499"
---
# <a name="uploadsession-resource"></a><span data-ttu-id="62c52-102">Recurso UploadSession</span><span class="sxs-lookup"><span data-stu-id="62c52-102">UploadSession resource</span></span>

> <span data-ttu-id="62c52-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="62c52-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="62c52-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="62c52-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="62c52-105">O recurso **UploadSession** fornece informações sobre como carregar arquivos grandes no OneDrive, no OneDrive for Business ou em bibliotecas de documentos do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="62c52-105">The **UploadSession** resource provides information about how to upload large files to OneDrive, OneDrive for Business, or SharePoint document libraries.</span></span>

## <a name="json-representation"></a><span data-ttu-id="62c52-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62c52-106">JSON representation</span></span>

<span data-ttu-id="62c52-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="62c52-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="62c52-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62c52-108">Properties</span></span>


| <span data-ttu-id="62c52-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62c52-109">Property</span></span>       | <span data-ttu-id="62c52-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="62c52-110">Type</span></span>              |<span data-ttu-id="62c52-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="62c52-111">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="62c52-112">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="62c52-112">expirationDateTime</span></span> | <span data-ttu-id="62c52-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62c52-113">DateTimeOffset</span></span>    | <span data-ttu-id="62c52-p102">Data e hora em UTC em que a sessão de carregamento expirará. O arquivo completo deve ser carregado antes que esta hora de expiração seja atingida.</span><span class="sxs-lookup"><span data-stu-id="62c52-p102">The date and time in UTC that the upload session will expire. The complete file must be uploaded before this expiration time is reached.</span></span>
| <span data-ttu-id="62c52-116">nextExpectedRanges</span><span class="sxs-lookup"><span data-stu-id="62c52-116">nextExpectedRanges</span></span> | <span data-ttu-id="62c52-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="62c52-117">String collection</span></span> | <span data-ttu-id="62c52-p103">Uma coleção de intervalos de bytes que estão ausentes do servidor para o arquivo. Estes intervalos são indexados como zero e têm o formato "início-fim" (por exemplo "0-26" para indicar os primeiros 27 bytes do arquivo).</span><span class="sxs-lookup"><span data-stu-id="62c52-p103">A collection of byte ranges that the server is missing for the file. These ranges are zero indexed and of the format "start-end" (e.g. "0-26" to indicate the first 27 bytes of the file).</span></span>
| <span data-ttu-id="62c52-120">uploadUrl</span><span class="sxs-lookup"><span data-stu-id="62c52-120">uploadUrl</span></span>          | <span data-ttu-id="62c52-121">String</span><span class="sxs-lookup"><span data-stu-id="62c52-121">String</span></span>            | <span data-ttu-id="62c52-122">O ponto de extremidade de URL que aceita solicitações PUT para intervalos de bytes do arquivo.</span><span class="sxs-lookup"><span data-stu-id="62c52-122">The URL endpoint that accepts PUT requests for byte ranges of the file.</span></span>

## <a name="see-also"></a><span data-ttu-id="62c52-123">Confira também</span><span class="sxs-lookup"><span data-stu-id="62c52-123">See also</span></span>

- [<span data-ttu-id="62c52-124">Carregar arquivos grandes em uma sessão de carregamento</span><span class="sxs-lookup"><span data-stu-id="62c52-124">Upload large files with an upload session</span></span>](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->
