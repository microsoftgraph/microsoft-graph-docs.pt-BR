---
title: Tipo de recurso referenceAttachment
description: Um link para um arquivo (como um arquivo de texto ou um documento do Word) em uma unidade de nuvem do OneDrive for Business ou outros locais de armazenamento compatíveis, anexado a um evento, mensagem ou postagem.
localization_priority: Normal
ms.prod: outlook
author: abheek-das
doc_type: resourcePageType
ms.openlocfilehash: ae16b7df05a6a240b0081e189d74b4622f2f7988
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129337"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="38691-103">Tipo de recurso referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="38691-103">referenceAttachment resource type</span></span>

<span data-ttu-id="38691-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38691-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="38691-105">Um link para um arquivo (como um arquivo de texto ou um documento do Word) em uma unidade de nuvem do OneDrive for Business ou outros locais de armazenamento compatíveis, anexado a um evento, mensagem ou postagem.</span><span class="sxs-lookup"><span data-stu-id="38691-105">A link to a file (such as a text file or Word document) on a OneDrive for Business cloud drive or other supported storage locations, attached to an event, message, or post.</span></span>

<span data-ttu-id="38691-106">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="38691-106">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="38691-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="38691-107">Methods</span></span>

| <span data-ttu-id="38691-108">Método</span><span class="sxs-lookup"><span data-stu-id="38691-108">Method</span></span>       | <span data-ttu-id="38691-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="38691-109">Return Type</span></span>  |<span data-ttu-id="38691-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="38691-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="38691-111">Get</span><span class="sxs-lookup"><span data-stu-id="38691-111">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="38691-112">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="38691-112">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="38691-113">Leia as propriedades e os relacionamentos do objeto referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="38691-113">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="38691-114">Delete</span><span class="sxs-lookup"><span data-stu-id="38691-114">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="38691-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="38691-115">None</span></span> |<span data-ttu-id="38691-116">Exclua o objeto referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="38691-116">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="38691-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38691-117">Properties</span></span>
| <span data-ttu-id="38691-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38691-118">Property</span></span>     | <span data-ttu-id="38691-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="38691-119">Type</span></span>   |<span data-ttu-id="38691-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="38691-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38691-121">contentType</span><span class="sxs-lookup"><span data-stu-id="38691-121">contentType</span></span>|<span data-ttu-id="38691-122">String</span><span class="sxs-lookup"><span data-stu-id="38691-122">String</span></span>|<span data-ttu-id="38691-123">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="38691-123">The content type of the attachment.</span></span>|
|<span data-ttu-id="38691-124">id</span><span class="sxs-lookup"><span data-stu-id="38691-124">id</span></span>|<span data-ttu-id="38691-125">String</span><span class="sxs-lookup"><span data-stu-id="38691-125">String</span></span>|<span data-ttu-id="38691-p101">A ID do anexo.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38691-p101">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="38691-128">isInline</span><span class="sxs-lookup"><span data-stu-id="38691-128">isInline</span></span>|<span data-ttu-id="38691-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="38691-129">Boolean</span></span>|<span data-ttu-id="38691-130">Defina como verdadeiro se o anexo é exibido embutido no corpo do objeto de incorporação.</span><span class="sxs-lookup"><span data-stu-id="38691-130">Set to true if the attachment appears inline in the body of the embedding object.</span></span>|
|<span data-ttu-id="38691-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38691-131">lastModifiedDateTime</span></span>|<span data-ttu-id="38691-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38691-132">DateTimeOffset</span></span>|<span data-ttu-id="38691-p102">Data e hora em que o anexo foi modificado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="38691-p102">The date and time when the attachment was last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="38691-136">nome</span><span class="sxs-lookup"><span data-stu-id="38691-136">name</span></span>|<span data-ttu-id="38691-137">String</span><span class="sxs-lookup"><span data-stu-id="38691-137">String</span></span>|<span data-ttu-id="38691-p103">O texto exibido abaixo do ícone que representa o anexo incorporado. Não precisa ser o nome real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="38691-p103">The text that is displayed below the icon representing the embedded attachment. This does not need to be the actual file name.</span></span>|
|<span data-ttu-id="38691-140">size</span><span class="sxs-lookup"><span data-stu-id="38691-140">size</span></span>|<span data-ttu-id="38691-141">Int32</span><span class="sxs-lookup"><span data-stu-id="38691-141">Int32</span></span>|<span data-ttu-id="38691-142">O tamanho dos metadados, em bytes, que são armazenados na mensagem para o anexo.</span><span class="sxs-lookup"><span data-stu-id="38691-142">The size of the metadata that is stored on the message for the attachment in bytes.</span></span> <span data-ttu-id="38691-143">Esse valor não indica o tamanho real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="38691-143">This value does not indicate the size of the actual file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38691-144">Relações</span><span class="sxs-lookup"><span data-stu-id="38691-144">Relationships</span></span>
<span data-ttu-id="38691-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="38691-145">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="38691-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38691-146">JSON representation</span></span>

<span data-ttu-id="38691-147">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="38691-147">Here is a JSON representation of the resource</span></span>

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

