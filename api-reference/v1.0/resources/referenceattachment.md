---
title: Tipo de recurso referenceAttachment
description: Um link para um arquivo (como um arquivo de texto ou um documento do Word) em uma unidade de nuvem do OneDrive for Business ou outros locais de armazenamento compatíveis, anexado a um evento, mensagem ou postagem.
localization_priority: Normal
ms.prod: outlook
author: angelgolfer-ms
doc_type: resourcePageType
ms.openlocfilehash: 49005be287e9ecb10bd184ff1c18750878fbaa46
ms.sourcegitcommit: 496269b62d42cb7a96752a77b0f2e0cb16918f0b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2019
ms.locfileid: "36484342"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="d3438-103">Tipo de recurso referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="d3438-103">referenceAttachment resource type</span></span>

<span data-ttu-id="d3438-104">Um link para um arquivo (como um arquivo de texto ou um documento do Word) em uma unidade de nuvem do OneDrive for Business ou outros locais de armazenamento compatíveis, anexado a um evento, mensagem ou postagem.</span><span class="sxs-lookup"><span data-stu-id="d3438-104">A link to a file (such as a text file or Word document) on a OneDrive for Business cloud drive or other supported storage locations, attached to an event, message, or post.</span></span>

<span data-ttu-id="d3438-105">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="d3438-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d3438-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="d3438-106">Methods</span></span>

| <span data-ttu-id="d3438-107">Método</span><span class="sxs-lookup"><span data-stu-id="d3438-107">Method</span></span>       | <span data-ttu-id="d3438-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d3438-108">Return Type</span></span>  |<span data-ttu-id="d3438-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3438-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d3438-110">Get</span><span class="sxs-lookup"><span data-stu-id="d3438-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="d3438-111">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="d3438-111">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="d3438-112">Leia as propriedades e os relacionamentos do objeto referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="d3438-112">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="d3438-113">Delete</span><span class="sxs-lookup"><span data-stu-id="d3438-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="d3438-114">None</span><span class="sxs-lookup"><span data-stu-id="d3438-114">None</span></span> |<span data-ttu-id="d3438-115">Exclua o objeto referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="d3438-115">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d3438-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3438-116">Properties</span></span>
| <span data-ttu-id="d3438-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3438-117">Property</span></span>     | <span data-ttu-id="d3438-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3438-118">Type</span></span>   |<span data-ttu-id="d3438-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3438-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3438-120">contentType</span><span class="sxs-lookup"><span data-stu-id="d3438-120">contentType</span></span>|<span data-ttu-id="d3438-121">String</span><span class="sxs-lookup"><span data-stu-id="d3438-121">String</span></span>|<span data-ttu-id="d3438-122">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="d3438-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="d3438-123">id</span><span class="sxs-lookup"><span data-stu-id="d3438-123">id</span></span>|<span data-ttu-id="d3438-124">String</span><span class="sxs-lookup"><span data-stu-id="d3438-124">String</span></span>|<span data-ttu-id="d3438-p101">A ID do anexo.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d3438-p101">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="d3438-127">isInline</span><span class="sxs-lookup"><span data-stu-id="d3438-127">isInline</span></span>|<span data-ttu-id="d3438-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="d3438-128">Boolean</span></span>|<span data-ttu-id="d3438-129">Defina como verdadeiro se o anexo é exibido embutido no corpo do objeto de incorporação.</span><span class="sxs-lookup"><span data-stu-id="d3438-129">Set to true if the attachment appears inline in the body of the embedding object.</span></span>|
|<span data-ttu-id="d3438-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3438-130">lastModifiedDateTime</span></span>|<span data-ttu-id="d3438-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3438-131">DateTimeOffset</span></span>|<span data-ttu-id="d3438-p102">Data e hora em que o anexo foi modificado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d3438-p102">The date and time when the attachment was last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d3438-135">name</span><span class="sxs-lookup"><span data-stu-id="d3438-135">name</span></span>|<span data-ttu-id="d3438-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3438-136">String</span></span>|<span data-ttu-id="d3438-p103">O texto exibido abaixo do ícone que representa o anexo incorporado. Não precisa ser o nome real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="d3438-p103">The text that is displayed below the icon representing the embedded attachment. This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="d3438-139">size</span><span class="sxs-lookup"><span data-stu-id="d3438-139">size</span></span>|<span data-ttu-id="d3438-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d3438-140">Int32</span></span>|<span data-ttu-id="d3438-141">O tamanho dos metadados, em bytes, que são armazenados na mensagem para o anexo.</span><span class="sxs-lookup"><span data-stu-id="d3438-141">The size of the metadata that is stored on the message for the attachment in bytes.</span></span> <span data-ttu-id="d3438-142">Esse valor não indica o tamanho real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="d3438-142">This value does not indicate the size of the actual file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3438-143">Relações</span><span class="sxs-lookup"><span data-stu-id="d3438-143">Relationships</span></span>
<span data-ttu-id="d3438-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d3438-144">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="d3438-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3438-145">JSON representation</span></span>

<span data-ttu-id="d3438-146">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d3438-146">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
