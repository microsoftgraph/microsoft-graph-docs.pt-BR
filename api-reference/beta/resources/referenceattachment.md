---
title: Tipo de recurso referenceAttachment
description: 'Um link para uma pasta ou arquivo (como um arquivo de texto ou documento do Word) em uma unidade de nuvem do OneDrive for Business ou outros locais de armazenamento com suporte, anexados a '
localization_priority: Normal
ms.openlocfilehash: 59ebb0af10a64195643cb7073d1206790ae6a875
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563071"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="80f90-103">Tipo de recurso referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="80f90-103">referenceAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80f90-104">Um link para uma pasta ou arquivo (como um arquivo de texto ou documento do Word) em uma unidade de nuvem do OneDrive for Business ou outros locais de armazenamento com suporte, anexados a um [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postagem](../resources/post.md) .</span><span class="sxs-lookup"><span data-stu-id="80f90-104">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="80f90-105">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="80f90-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="80f90-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="80f90-106">Methods</span></span>

| <span data-ttu-id="80f90-107">Método</span><span class="sxs-lookup"><span data-stu-id="80f90-107">Method</span></span>       | <span data-ttu-id="80f90-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="80f90-108">Return Type</span></span>  |<span data-ttu-id="80f90-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="80f90-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="80f90-110">Get</span><span class="sxs-lookup"><span data-stu-id="80f90-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="80f90-111">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="80f90-111">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="80f90-112">Leia as propriedades e os relacionamentos do objeto referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="80f90-112">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="80f90-113">Excluir</span><span class="sxs-lookup"><span data-stu-id="80f90-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="80f90-114">None</span><span class="sxs-lookup"><span data-stu-id="80f90-114">None</span></span> |<span data-ttu-id="80f90-115">Exclua o objeto referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="80f90-115">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="80f90-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80f90-116">Properties</span></span>
| <span data-ttu-id="80f90-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80f90-117">Property</span></span>     | <span data-ttu-id="80f90-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="80f90-118">Type</span></span>   |<span data-ttu-id="80f90-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="80f90-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80f90-120">contentType</span><span class="sxs-lookup"><span data-stu-id="80f90-120">contentType</span></span>|<span data-ttu-id="80f90-121">String</span><span class="sxs-lookup"><span data-stu-id="80f90-121">String</span></span>|<span data-ttu-id="80f90-122">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="80f90-122">The content type of the attachment.</span></span> <span data-ttu-id="80f90-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="80f90-123">Optional.</span></span>|
|<span data-ttu-id="80f90-124">id</span><span class="sxs-lookup"><span data-stu-id="80f90-124">id</span></span>|<span data-ttu-id="80f90-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80f90-125">String</span></span>|<span data-ttu-id="80f90-p102">A ID do anexo.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80f90-p102">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="80f90-128">isFolder</span><span class="sxs-lookup"><span data-stu-id="80f90-128">isFolder</span></span>|<span data-ttu-id="80f90-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="80f90-129">Boolean</span></span>|<span data-ttu-id="80f90-130">Especifica se o anexo é um link para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="80f90-130">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="80f90-131">Deve definir this como true se **sourceUrl** for um link para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="80f90-131">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="80f90-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="80f90-132">Optional.</span></span>|
|<span data-ttu-id="80f90-133">isInline</span><span class="sxs-lookup"><span data-stu-id="80f90-133">isInline</span></span>|<span data-ttu-id="80f90-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="80f90-134">Boolean</span></span>|<span data-ttu-id="80f90-135">Defina como verdadeiro se o anexo é exibido embutido no corpo do objeto de incorporação.</span><span class="sxs-lookup"><span data-stu-id="80f90-135">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="80f90-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="80f90-136">Optional.</span></span>|
|<span data-ttu-id="80f90-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80f90-137">lastModifiedDateTime</span></span>|<span data-ttu-id="80f90-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80f90-138">DateTimeOffset</span></span>|<span data-ttu-id="80f90-139">Data e hora em que o anexo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="80f90-139">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="80f90-140">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="80f90-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="80f90-141">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="80f90-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="80f90-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="80f90-142">Optional.</span></span>|
|<span data-ttu-id="80f90-143">name</span><span class="sxs-lookup"><span data-stu-id="80f90-143">name</span></span>|<span data-ttu-id="80f90-144">String</span><span class="sxs-lookup"><span data-stu-id="80f90-144">String</span></span>|<span data-ttu-id="80f90-145">O texto exibido abaixo do ícone que representa o anexo incorporado.</span><span class="sxs-lookup"><span data-stu-id="80f90-145">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="80f90-146">Não precisa ser o nome real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="80f90-146">This does not need to be the actual file name.</span></span> <span data-ttu-id="80f90-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80f90-147">Required.</span></span>|
|<span data-ttu-id="80f90-148">autorização</span><span class="sxs-lookup"><span data-stu-id="80f90-148">permission</span></span>|<span data-ttu-id="80f90-149">ReferenceAttachmentPermissions</span><span class="sxs-lookup"><span data-stu-id="80f90-149">ReferenceAttachmentPermissions</span></span>|<span data-ttu-id="80f90-150">Especifica as permissões concedidas para o anexo pelo tipo de provedor no **ProviderType**.</span><span class="sxs-lookup"><span data-stu-id="80f90-150">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="80f90-151">Os valores possíveis são: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span><span class="sxs-lookup"><span data-stu-id="80f90-151">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="80f90-152">Opcional.</span><span class="sxs-lookup"><span data-stu-id="80f90-152">Optional.</span></span>|
|<span data-ttu-id="80f90-153">previewUrl</span><span class="sxs-lookup"><span data-stu-id="80f90-153">previewUrl</span></span>|<span data-ttu-id="80f90-154">String</span><span class="sxs-lookup"><span data-stu-id="80f90-154">String</span></span>|<span data-ttu-id="80f90-155">Aplica-se somente a um anexo de referência de uma URL de imagem para obter uma imagem de visualização.</span><span class="sxs-lookup"><span data-stu-id="80f90-155">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="80f90-156">Use **thumbnailUrl** e **PreviewUrl** somente quando **sourceUrl** identifica um arquivo de imagem.</span><span class="sxs-lookup"><span data-stu-id="80f90-156">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="80f90-157">Opcional.</span><span class="sxs-lookup"><span data-stu-id="80f90-157">Optional.</span></span>|
|<span data-ttu-id="80f90-158">providerType</span><span class="sxs-lookup"><span data-stu-id="80f90-158">providerType</span></span>|<span data-ttu-id="80f90-159">ReferenceAttachmentProviders</span><span class="sxs-lookup"><span data-stu-id="80f90-159">ReferenceAttachmentProviders</span></span>|<span data-ttu-id="80f90-160">O tipo de provedor que dá suporte a um anexo deste contentType.</span><span class="sxs-lookup"><span data-stu-id="80f90-160">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="80f90-161">Os valores possíveis são: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span><span class="sxs-lookup"><span data-stu-id="80f90-161">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="80f90-162">Opcional.</span><span class="sxs-lookup"><span data-stu-id="80f90-162">Optional.</span></span>|
|<span data-ttu-id="80f90-163">size</span><span class="sxs-lookup"><span data-stu-id="80f90-163">size</span></span>|<span data-ttu-id="80f90-164">Int32</span><span class="sxs-lookup"><span data-stu-id="80f90-164">Int32</span></span>|<span data-ttu-id="80f90-165">O tamanho dos metadados em bytes armazenados na mensagem para o anexo de referência.</span><span class="sxs-lookup"><span data-stu-id="80f90-165">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="80f90-166">Esse valor não indica o tamanho real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="80f90-166">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="80f90-167">Opcional.</span><span class="sxs-lookup"><span data-stu-id="80f90-167">Optional.</span></span>|
|<span data-ttu-id="80f90-168">Urlorigem</span><span class="sxs-lookup"><span data-stu-id="80f90-168">sourceUrl</span></span>|<span data-ttu-id="80f90-169">String</span><span class="sxs-lookup"><span data-stu-id="80f90-169">String</span></span>|<span data-ttu-id="80f90-170">URL para obter o conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="80f90-170">URL to get the attachment content.</span></span> <span data-ttu-id="80f90-171">Se esta for uma URL para uma pasta, para que a pasta seja exibida corretamente no Outlook ou no Outlook na Web, defina **IsFolder** como true.</span><span class="sxs-lookup"><span data-stu-id="80f90-171">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="80f90-172">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80f90-172">Required.</span></span>|
|<span data-ttu-id="80f90-173">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="80f90-173">thumbnailUrl</span></span>|<span data-ttu-id="80f90-174">String</span><span class="sxs-lookup"><span data-stu-id="80f90-174">String</span></span>|<span data-ttu-id="80f90-175">Aplica-se somente a um anexo de referência de uma URL de imagem para obter uma imagem em miniatura.</span><span class="sxs-lookup"><span data-stu-id="80f90-175">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="80f90-176">Use **thumbnailUrl** e **PreviewUrl** somente quando **sourceUrl** identifica um arquivo de imagem.</span><span class="sxs-lookup"><span data-stu-id="80f90-176">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="80f90-177">Opcional.</span><span class="sxs-lookup"><span data-stu-id="80f90-177">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80f90-178">Relações</span><span class="sxs-lookup"><span data-stu-id="80f90-178">Relationships</span></span>
<span data-ttu-id="80f90-179">Nenhum</span><span class="sxs-lookup"><span data-stu-id="80f90-179">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="80f90-180">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80f90-180">JSON representation</span></span>

<span data-ttu-id="80f90-181">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="80f90-181">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/referenceattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
