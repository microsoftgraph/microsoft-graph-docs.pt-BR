---
title: Tipo de recurso referenceAttachment
description: 'Um link para uma pasta ou arquivo (por exemplo, um arquivo de texto ou um documento do Word) em um OneDrive para a unidade de nuvem de negócios ou outros locais de armazenamento suportadas, anexado ao '
localization_priority: Normal
ms.openlocfilehash: adf078f7ba678a4fe90a51972c5e4be4788c9c0c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574555"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="33cbc-103">Tipo de recurso referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="33cbc-103">referenceAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33cbc-104">Um link para uma pasta ou um arquivo (por exemplo, um arquivo de texto ou um documento do Word) em um OneDrive para Business cloud unidade ou outro suporte para locais de armazenamento anexados a um [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postar](../resources/post.md) .</span><span class="sxs-lookup"><span data-stu-id="33cbc-104">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="33cbc-105">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="33cbc-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="33cbc-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="33cbc-106">Methods</span></span>

| <span data-ttu-id="33cbc-107">Método</span><span class="sxs-lookup"><span data-stu-id="33cbc-107">Method</span></span>       | <span data-ttu-id="33cbc-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="33cbc-108">Return Type</span></span>  |<span data-ttu-id="33cbc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="33cbc-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="33cbc-110">Get</span><span class="sxs-lookup"><span data-stu-id="33cbc-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="33cbc-111">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="33cbc-111">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="33cbc-112">Leia as propriedades e os relacionamentos do objeto referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="33cbc-112">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="33cbc-113">Delete</span><span class="sxs-lookup"><span data-stu-id="33cbc-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="33cbc-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="33cbc-114">None</span></span> |<span data-ttu-id="33cbc-115">Exclua o objeto referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="33cbc-115">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="33cbc-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="33cbc-116">Properties</span></span>
| <span data-ttu-id="33cbc-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33cbc-117">Property</span></span>     | <span data-ttu-id="33cbc-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="33cbc-118">Type</span></span>   |<span data-ttu-id="33cbc-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="33cbc-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33cbc-120">contentType</span><span class="sxs-lookup"><span data-stu-id="33cbc-120">contentType</span></span>|<span data-ttu-id="33cbc-121">String</span><span class="sxs-lookup"><span data-stu-id="33cbc-121">String</span></span>|<span data-ttu-id="33cbc-122">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="33cbc-122">The content type of the attachment.</span></span> <span data-ttu-id="33cbc-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="33cbc-123">Optional.</span></span>|
|<span data-ttu-id="33cbc-124">id</span><span class="sxs-lookup"><span data-stu-id="33cbc-124">id</span></span>|<span data-ttu-id="33cbc-125">String</span><span class="sxs-lookup"><span data-stu-id="33cbc-125">String</span></span>|<span data-ttu-id="33cbc-p102">A ID do anexo.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="33cbc-p102">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="33cbc-128">isFolder</span><span class="sxs-lookup"><span data-stu-id="33cbc-128">isFolder</span></span>|<span data-ttu-id="33cbc-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="33cbc-129">Boolean</span></span>|<span data-ttu-id="33cbc-130">Especifica se o anexo é um link para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="33cbc-130">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="33cbc-131">Defina essa opção para true se **sourceUrl** é um link para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="33cbc-131">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="33cbc-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="33cbc-132">Optional.</span></span>|
|<span data-ttu-id="33cbc-133">isInline</span><span class="sxs-lookup"><span data-stu-id="33cbc-133">isInline</span></span>|<span data-ttu-id="33cbc-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="33cbc-134">Boolean</span></span>|<span data-ttu-id="33cbc-135">Defina como verdadeiro se o anexo é exibido embutido no corpo do objeto de incorporação.</span><span class="sxs-lookup"><span data-stu-id="33cbc-135">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="33cbc-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="33cbc-136">Optional.</span></span>|
|<span data-ttu-id="33cbc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33cbc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="33cbc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33cbc-138">DateTimeOffset</span></span>|<span data-ttu-id="33cbc-139">Data e hora em que o anexo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="33cbc-139">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="33cbc-140">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="33cbc-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="33cbc-141">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="33cbc-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="33cbc-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="33cbc-142">Optional.</span></span>|
|<span data-ttu-id="33cbc-143">name</span><span class="sxs-lookup"><span data-stu-id="33cbc-143">name</span></span>|<span data-ttu-id="33cbc-144">String</span><span class="sxs-lookup"><span data-stu-id="33cbc-144">String</span></span>|<span data-ttu-id="33cbc-145">O texto que é exibido abaixo do ícone que representa o anexo incorporado.</span><span class="sxs-lookup"><span data-stu-id="33cbc-145">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="33cbc-146">Isso não precisa ser o nome de arquivo real.</span><span class="sxs-lookup"><span data-stu-id="33cbc-146">This does not need to be the actual file name.</span></span> <span data-ttu-id="33cbc-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33cbc-147">Required.</span></span>|
|<span data-ttu-id="33cbc-148">permissão</span><span class="sxs-lookup"><span data-stu-id="33cbc-148">permission</span></span>|<span data-ttu-id="33cbc-149">referenceAttachmentPermission</span><span class="sxs-lookup"><span data-stu-id="33cbc-149">referenceAttachmentPermission</span></span>|<span data-ttu-id="33cbc-150">Especifica as permissões concedidas pelo tipo de provedor na **providerType**o anexo.</span><span class="sxs-lookup"><span data-stu-id="33cbc-150">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="33cbc-151">Os valores possíveis são: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span><span class="sxs-lookup"><span data-stu-id="33cbc-151">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="33cbc-152">Opcional.</span><span class="sxs-lookup"><span data-stu-id="33cbc-152">Optional.</span></span>|
|<span data-ttu-id="33cbc-153">previewUrl</span><span class="sxs-lookup"><span data-stu-id="33cbc-153">previewUrl</span></span>|<span data-ttu-id="33cbc-154">String</span><span class="sxs-lookup"><span data-stu-id="33cbc-154">String</span></span>|<span data-ttu-id="33cbc-155">Se aplica a apenas um anexo de referência de uma imagem - URL para obter uma imagem de visualização.</span><span class="sxs-lookup"><span data-stu-id="33cbc-155">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="33cbc-156">Use **thumbnailUrl** e **previewUrl** somente quando **sourceUrl** identifica um arquivo de imagem.</span><span class="sxs-lookup"><span data-stu-id="33cbc-156">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="33cbc-157">Opcional.</span><span class="sxs-lookup"><span data-stu-id="33cbc-157">Optional.</span></span>|
|<span data-ttu-id="33cbc-158">providerType</span><span class="sxs-lookup"><span data-stu-id="33cbc-158">providerType</span></span>| <span data-ttu-id="33cbc-159">referenceAttachmentProvider</span><span class="sxs-lookup"><span data-stu-id="33cbc-159">referenceAttachmentProvider</span></span> |<span data-ttu-id="33cbc-160">O tipo de provedor que ofereça suporte a um anexo deste contentType.</span><span class="sxs-lookup"><span data-stu-id="33cbc-160">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="33cbc-161">Os valores possíveis são: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span><span class="sxs-lookup"><span data-stu-id="33cbc-161">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="33cbc-162">Opcional.</span><span class="sxs-lookup"><span data-stu-id="33cbc-162">Optional.</span></span>|
|<span data-ttu-id="33cbc-163">size</span><span class="sxs-lookup"><span data-stu-id="33cbc-163">size</span></span>|<span data-ttu-id="33cbc-164">Int32</span><span class="sxs-lookup"><span data-stu-id="33cbc-164">Int32</span></span>|<span data-ttu-id="33cbc-165">O tamanho dos metadados em bytes que é armazenado na mensagem do anexo da referência.</span><span class="sxs-lookup"><span data-stu-id="33cbc-165">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="33cbc-166">Esse valor não indica o tamanho real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="33cbc-166">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="33cbc-167">Opcional.</span><span class="sxs-lookup"><span data-stu-id="33cbc-167">Optional.</span></span>|
|<span data-ttu-id="33cbc-168">Urlorigem</span><span class="sxs-lookup"><span data-stu-id="33cbc-168">sourceUrl</span></span>|<span data-ttu-id="33cbc-169">String</span><span class="sxs-lookup"><span data-stu-id="33cbc-169">String</span></span>|<span data-ttu-id="33cbc-170">URL para obter o conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="33cbc-170">URL to get the attachment content.</span></span> <span data-ttu-id="33cbc-171">Se essa for uma URL para uma pasta, em seguida, para a pasta para serem exibidos corretamente no Outlook ou no Outlook na web, defina **isFolder** como true.</span><span class="sxs-lookup"><span data-stu-id="33cbc-171">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="33cbc-172">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33cbc-172">Required.</span></span>|
|<span data-ttu-id="33cbc-173">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="33cbc-173">thumbnailUrl</span></span>|<span data-ttu-id="33cbc-174">String</span><span class="sxs-lookup"><span data-stu-id="33cbc-174">String</span></span>|<span data-ttu-id="33cbc-175">Se aplica a apenas um anexo de referência de uma imagem - URL para obter uma imagem em miniatura.</span><span class="sxs-lookup"><span data-stu-id="33cbc-175">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="33cbc-176">Use **thumbnailUrl** e **previewUrl** somente quando **sourceUrl** identifica um arquivo de imagem.</span><span class="sxs-lookup"><span data-stu-id="33cbc-176">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="33cbc-177">Opcional.</span><span class="sxs-lookup"><span data-stu-id="33cbc-177">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33cbc-178">Relações</span><span class="sxs-lookup"><span data-stu-id="33cbc-178">Relationships</span></span>
<span data-ttu-id="33cbc-179">Nenhum</span><span class="sxs-lookup"><span data-stu-id="33cbc-179">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="33cbc-180">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="33cbc-180">JSON representation</span></span>

<span data-ttu-id="33cbc-181">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="33cbc-181">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
  "permission": "referenceAttachmentPermission",
  "previewUrl": "string",
  "providerType": "referenceAttachmentProvider",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/referenceattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
