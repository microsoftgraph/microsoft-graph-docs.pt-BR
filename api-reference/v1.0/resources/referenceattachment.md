---
title: Tipo de recurso referenceAttachment
description: Um link para um arquivo (como um arquivo de texto ou um documento do Word) em uma unidade de nuvem do OneDrive for Business ou outros locais de armazenamento compatíveis, anexado a um evento, mensagem ou postagem.
localization_priority: Normal
ms.openlocfilehash: 0696ac4b0f93ed4982ec576a15afe071486f9c88
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853120"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="890d3-103">Tipo de recurso referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="890d3-103">referenceAttachment resource type</span></span>

<span data-ttu-id="890d3-104">Um link para um arquivo (como um arquivo de texto ou um documento do Word) em uma unidade de nuvem do OneDrive for Business ou outros locais de armazenamento compatíveis, anexado a um evento, mensagem ou postagem.</span><span class="sxs-lookup"><span data-stu-id="890d3-104">A link to a file (such as a text file or Word document) on a OneDrive for Business cloud drive or other supported storage locations, attached to an event, message, or post.</span></span>

<span data-ttu-id="890d3-105">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="890d3-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="890d3-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="890d3-106">Methods</span></span>

| <span data-ttu-id="890d3-107">Método</span><span class="sxs-lookup"><span data-stu-id="890d3-107">Method</span></span>       | <span data-ttu-id="890d3-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="890d3-108">Return Type</span></span>  |<span data-ttu-id="890d3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="890d3-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="890d3-110">Get</span><span class="sxs-lookup"><span data-stu-id="890d3-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="890d3-111">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="890d3-111">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="890d3-112">Leia as propriedades e os relacionamentos do objeto referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="890d3-112">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="890d3-113">Delete</span><span class="sxs-lookup"><span data-stu-id="890d3-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="890d3-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="890d3-114">None</span></span> |<span data-ttu-id="890d3-115">Exclua o objeto referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="890d3-115">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="890d3-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="890d3-116">Properties</span></span>
| <span data-ttu-id="890d3-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="890d3-117">Property</span></span>     | <span data-ttu-id="890d3-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="890d3-118">Type</span></span>   |<span data-ttu-id="890d3-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="890d3-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="890d3-120">contentType</span><span class="sxs-lookup"><span data-stu-id="890d3-120">contentType</span></span>|<span data-ttu-id="890d3-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="890d3-121">String</span></span>|<span data-ttu-id="890d3-122">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="890d3-122">The content type of the attachment.</span></span>|
|<span data-ttu-id="890d3-123">id</span><span class="sxs-lookup"><span data-stu-id="890d3-123">id</span></span>|<span data-ttu-id="890d3-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="890d3-124">String</span></span>|<span data-ttu-id="890d3-p101">A ID do anexo.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="890d3-p101">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="890d3-127">isInline</span><span class="sxs-lookup"><span data-stu-id="890d3-127">isInline</span></span>|<span data-ttu-id="890d3-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="890d3-128">Boolean</span></span>|<span data-ttu-id="890d3-129">Defina como verdadeiro se o anexo é exibido embutido no corpo do objeto de incorporação.</span><span class="sxs-lookup"><span data-stu-id="890d3-129">Set to true if the attachment appears inline in the body of the embedding object.</span></span>|
|<span data-ttu-id="890d3-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="890d3-130">lastModifiedDateTime</span></span>|<span data-ttu-id="890d3-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="890d3-131">DateTimeOffset</span></span>|<span data-ttu-id="890d3-p102">Data e hora em que o anexo foi modificado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="890d3-p102">The date and time when the attachment was last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="890d3-135">nome</span><span class="sxs-lookup"><span data-stu-id="890d3-135">name</span></span>|<span data-ttu-id="890d3-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="890d3-136">String</span></span>|<span data-ttu-id="890d3-p103">O texto exibido abaixo do ícone que representa o anexo incorporado. Não precisa ser o nome real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="890d3-p103">The text that is displayed below the icon representing the embedded attachment. This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="890d3-139">size</span><span class="sxs-lookup"><span data-stu-id="890d3-139">size</span></span>|<span data-ttu-id="890d3-140">Int32</span><span class="sxs-lookup"><span data-stu-id="890d3-140">Int32</span></span>|<span data-ttu-id="890d3-141">O tamanho dos metadados, em bytes, que são armazenados na mensagem para o anexo.</span><span class="sxs-lookup"><span data-stu-id="890d3-141">The size of the metadata that is stored on the message for the attachment in bytes.</span></span> <span data-ttu-id="890d3-142">Esse valor não indica o tamanho real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="890d3-142">This value does not indicate the size of the actual file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="890d3-143">Relações</span><span class="sxs-lookup"><span data-stu-id="890d3-143">Relationships</span></span>
<span data-ttu-id="890d3-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="890d3-144">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="890d3-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="890d3-145">JSON representation</span></span>

<span data-ttu-id="890d3-146">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="890d3-146">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.attachment",
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
