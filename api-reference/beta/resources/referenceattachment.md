---
title: Tipo de recurso referenceAttachment
description: 'Um link para uma pasta ou arquivo (como um arquivo de texto ou documento do Word) em uma unidade de nuvem do OneDrive for Business ou outros locais de armazenamento com suporte anexados a '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 914d04a6482b96fda0ee55c92f25bf950e594173
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136763"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="481c5-103">Tipo de recurso referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="481c5-103">referenceAttachment resource type</span></span>

<span data-ttu-id="481c5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="481c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="481c5-105">Um link para uma pasta ou arquivo (como um arquivo de texto ou documento do Word) em uma [](../resources/message.md)unidade de nuvem do OneDrive for Business ou outros locais de armazenamento com suporte, anexados a um [evento,](../resources/event.md)mensagem ou [postagem.](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="481c5-105">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="481c5-106">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="481c5-106">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="481c5-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="481c5-107">Methods</span></span>

| <span data-ttu-id="481c5-108">Método</span><span class="sxs-lookup"><span data-stu-id="481c5-108">Method</span></span>       | <span data-ttu-id="481c5-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="481c5-109">Return Type</span></span>  |<span data-ttu-id="481c5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="481c5-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="481c5-111">Get</span><span class="sxs-lookup"><span data-stu-id="481c5-111">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="481c5-112">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="481c5-112">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="481c5-113">Leia as propriedades e os relacionamentos do objeto referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="481c5-113">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="481c5-114">Delete</span><span class="sxs-lookup"><span data-stu-id="481c5-114">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="481c5-115">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="481c5-115">None</span></span> |<span data-ttu-id="481c5-116">Exclua o objeto referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="481c5-116">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="481c5-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="481c5-117">Properties</span></span>
| <span data-ttu-id="481c5-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="481c5-118">Property</span></span>     | <span data-ttu-id="481c5-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="481c5-119">Type</span></span>   |<span data-ttu-id="481c5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="481c5-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="481c5-121">contentType</span><span class="sxs-lookup"><span data-stu-id="481c5-121">contentType</span></span>|<span data-ttu-id="481c5-122">String</span><span class="sxs-lookup"><span data-stu-id="481c5-122">String</span></span>|<span data-ttu-id="481c5-123">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="481c5-123">The content type of the attachment.</span></span> <span data-ttu-id="481c5-124">Opcional.</span><span class="sxs-lookup"><span data-stu-id="481c5-124">Optional.</span></span>|
|<span data-ttu-id="481c5-125">id</span><span class="sxs-lookup"><span data-stu-id="481c5-125">id</span></span>|<span data-ttu-id="481c5-126">String</span><span class="sxs-lookup"><span data-stu-id="481c5-126">String</span></span>|<span data-ttu-id="481c5-p102">A ID do anexo.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="481c5-p102">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="481c5-129">isFolder</span><span class="sxs-lookup"><span data-stu-id="481c5-129">isFolder</span></span>|<span data-ttu-id="481c5-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="481c5-130">Boolean</span></span>|<span data-ttu-id="481c5-131">Especifica se o anexo é um link para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="481c5-131">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="481c5-132">Deve definir isso como true se **sourceUrl** for um link para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="481c5-132">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="481c5-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="481c5-133">Optional.</span></span>|
|<span data-ttu-id="481c5-134">isInline</span><span class="sxs-lookup"><span data-stu-id="481c5-134">isInline</span></span>|<span data-ttu-id="481c5-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="481c5-135">Boolean</span></span>|<span data-ttu-id="481c5-136">Defina como verdadeiro se o anexo é exibido embutido no corpo do objeto de incorporação.</span><span class="sxs-lookup"><span data-stu-id="481c5-136">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="481c5-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="481c5-137">Optional.</span></span>|
|<span data-ttu-id="481c5-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="481c5-138">lastModifiedDateTime</span></span>|<span data-ttu-id="481c5-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="481c5-139">DateTimeOffset</span></span>|<span data-ttu-id="481c5-140">Data e hora em que o anexo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="481c5-140">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="481c5-141">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="481c5-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="481c5-142">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="481c5-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="481c5-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="481c5-143">Optional.</span></span>|
|<span data-ttu-id="481c5-144">nome</span><span class="sxs-lookup"><span data-stu-id="481c5-144">name</span></span>|<span data-ttu-id="481c5-145">String</span><span class="sxs-lookup"><span data-stu-id="481c5-145">String</span></span>|<span data-ttu-id="481c5-146">O texto exibido abaixo do ícone que representa o anexo incorporado.</span><span class="sxs-lookup"><span data-stu-id="481c5-146">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="481c5-147">Não precisa ser o nome real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="481c5-147">This does not need to be the actual file name.</span></span> <span data-ttu-id="481c5-148">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="481c5-148">Required.</span></span>|
|<span data-ttu-id="481c5-149">permission</span><span class="sxs-lookup"><span data-stu-id="481c5-149">permission</span></span>|<span data-ttu-id="481c5-150">referenceAttachmentPermission</span><span class="sxs-lookup"><span data-stu-id="481c5-150">referenceAttachmentPermission</span></span>|<span data-ttu-id="481c5-151">Especifica as permissões concedidas para o anexo pelo tipo de provedor em **providerType**.</span><span class="sxs-lookup"><span data-stu-id="481c5-151">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="481c5-152">Os valores possíveis são: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span><span class="sxs-lookup"><span data-stu-id="481c5-152">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="481c5-153">Opcional.</span><span class="sxs-lookup"><span data-stu-id="481c5-153">Optional.</span></span>|
|<span data-ttu-id="481c5-154">previewUrl</span><span class="sxs-lookup"><span data-stu-id="481c5-154">previewUrl</span></span>|<span data-ttu-id="481c5-155">String</span><span class="sxs-lookup"><span data-stu-id="481c5-155">String</span></span>|<span data-ttu-id="481c5-156">Aplica-se apenas a um anexo de referência de uma imagem - URL para obter uma imagem de visualização.</span><span class="sxs-lookup"><span data-stu-id="481c5-156">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="481c5-157">Use **thumbnailUrl** e **previewUrl** somente quando **sourceUrl** identificar um arquivo de imagem.</span><span class="sxs-lookup"><span data-stu-id="481c5-157">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="481c5-158">Opcional.</span><span class="sxs-lookup"><span data-stu-id="481c5-158">Optional.</span></span>|
|<span data-ttu-id="481c5-159">providerType</span><span class="sxs-lookup"><span data-stu-id="481c5-159">providerType</span></span>|<span data-ttu-id="481c5-160">referenceAttachmentProvider</span><span class="sxs-lookup"><span data-stu-id="481c5-160">referenceAttachmentProvider</span></span>|<span data-ttu-id="481c5-161">O tipo de provedor que oferece suporte a um anexo desse contentType.</span><span class="sxs-lookup"><span data-stu-id="481c5-161">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="481c5-162">Os valores possíveis são: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span><span class="sxs-lookup"><span data-stu-id="481c5-162">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="481c5-163">Opcional.</span><span class="sxs-lookup"><span data-stu-id="481c5-163">Optional.</span></span>|
|<span data-ttu-id="481c5-164">size</span><span class="sxs-lookup"><span data-stu-id="481c5-164">size</span></span>|<span data-ttu-id="481c5-165">Int32</span><span class="sxs-lookup"><span data-stu-id="481c5-165">Int32</span></span>|<span data-ttu-id="481c5-166">O tamanho dos metadados em bytes armazenados na mensagem para o anexo de referência.</span><span class="sxs-lookup"><span data-stu-id="481c5-166">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="481c5-167">Esse valor não indica o tamanho real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="481c5-167">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="481c5-168">Opcional.</span><span class="sxs-lookup"><span data-stu-id="481c5-168">Optional.</span></span>|
|<span data-ttu-id="481c5-169">Urlorigem</span><span class="sxs-lookup"><span data-stu-id="481c5-169">sourceUrl</span></span>|<span data-ttu-id="481c5-170">String</span><span class="sxs-lookup"><span data-stu-id="481c5-170">String</span></span>|<span data-ttu-id="481c5-171">URL para obter o conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="481c5-171">URL to get the attachment content.</span></span> <span data-ttu-id="481c5-172">Se for uma URL para uma pasta, para que a pasta seja exibida corretamente no Outlook ou no Outlook na Web, de definida como true **isFolder.**</span><span class="sxs-lookup"><span data-stu-id="481c5-172">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="481c5-173">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="481c5-173">Required.</span></span>|
|<span data-ttu-id="481c5-174">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="481c5-174">thumbnailUrl</span></span>|<span data-ttu-id="481c5-175">String</span><span class="sxs-lookup"><span data-stu-id="481c5-175">String</span></span>|<span data-ttu-id="481c5-176">Aplica-se apenas a um anexo de referência de uma imagem - URL para obter uma imagem em miniatura.</span><span class="sxs-lookup"><span data-stu-id="481c5-176">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="481c5-177">Use **thumbnailUrl** e **previewUrl** somente quando **sourceUrl** identificar um arquivo de imagem.</span><span class="sxs-lookup"><span data-stu-id="481c5-177">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="481c5-178">Opcional.</span><span class="sxs-lookup"><span data-stu-id="481c5-178">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="481c5-179">Relações</span><span class="sxs-lookup"><span data-stu-id="481c5-179">Relationships</span></span>
<span data-ttu-id="481c5-180">Nenhum</span><span class="sxs-lookup"><span data-stu-id="481c5-180">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="481c5-181">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="481c5-181">JSON representation</span></span>

<span data-ttu-id="481c5-182">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="481c5-182">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isFolder": true,
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "permission": "string",
  "previewUrl": "string",
  "providerType": "string",
  "size": 1024,
  "sourceUrl": "string",
  "thumbnailUrl": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


