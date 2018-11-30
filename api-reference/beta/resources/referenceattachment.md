---
title: Tipo de recurso referenceAttachment
description: 'Um link para uma pasta ou arquivo (por exemplo, um arquivo de texto ou um documento do Word) em um OneDrive para a unidade de nuvem de negócios ou outros locais de armazenamento suportadas, anexado ao '
ms.openlocfilehash: e9885c3a0e5c7f723303d7d6461f4c07dbed6bf6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038916"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="c011d-103">Tipo de recurso referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="c011d-103">referenceAttachment resource type</span></span>

> <span data-ttu-id="c011d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c011d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c011d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c011d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c011d-106">Um link para uma pasta ou um arquivo (por exemplo, um arquivo de texto ou um documento do Word) em um OneDrive para Business cloud unidade ou outro suporte para locais de armazenamento anexados a um [evento](../resources/event.md), [mensagem](../resources/message.md), [tarefa do Outlook](../resources/outlooktask.md)ou [postar](../resources/post.md) .</span><span class="sxs-lookup"><span data-stu-id="c011d-106">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="c011d-107">Derivado de [attachment](attachment.md).</span><span class="sxs-lookup"><span data-stu-id="c011d-107">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c011d-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="c011d-108">Methods</span></span>

| <span data-ttu-id="c011d-109">Método</span><span class="sxs-lookup"><span data-stu-id="c011d-109">Method</span></span>       | <span data-ttu-id="c011d-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c011d-110">Return Type</span></span>  |<span data-ttu-id="c011d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c011d-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c011d-112">Get</span><span class="sxs-lookup"><span data-stu-id="c011d-112">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="c011d-113">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="c011d-113">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="c011d-114">Leia as propriedades e os relacionamentos do objeto referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="c011d-114">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="c011d-115">Delete</span><span class="sxs-lookup"><span data-stu-id="c011d-115">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="c011d-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c011d-116">None</span></span> |<span data-ttu-id="c011d-117">Exclua o objeto referenceAttachment.</span><span class="sxs-lookup"><span data-stu-id="c011d-117">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c011d-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c011d-118">Properties</span></span>
| <span data-ttu-id="c011d-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c011d-119">Property</span></span>     | <span data-ttu-id="c011d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="c011d-120">Type</span></span>   |<span data-ttu-id="c011d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c011d-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c011d-122">contentType</span><span class="sxs-lookup"><span data-stu-id="c011d-122">contentType</span></span>|<span data-ttu-id="c011d-123">String</span><span class="sxs-lookup"><span data-stu-id="c011d-123">String</span></span>|<span data-ttu-id="c011d-124">O tipo de conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="c011d-124">The content type of the attachment.</span></span> <span data-ttu-id="c011d-125">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c011d-125">Optional.</span></span>|
|<span data-ttu-id="c011d-126">id</span><span class="sxs-lookup"><span data-stu-id="c011d-126">id</span></span>|<span data-ttu-id="c011d-127">String</span><span class="sxs-lookup"><span data-stu-id="c011d-127">String</span></span>|<span data-ttu-id="c011d-p103">A ID do anexo.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c011d-p103">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="c011d-130">isFolder</span><span class="sxs-lookup"><span data-stu-id="c011d-130">isFolder</span></span>|<span data-ttu-id="c011d-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="c011d-131">Boolean</span></span>|<span data-ttu-id="c011d-132">Especifica se o anexo é um link para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="c011d-132">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="c011d-133">Defina essa opção para true se **sourceUrl** é um link para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="c011d-133">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="c011d-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c011d-134">Optional.</span></span>|
|<span data-ttu-id="c011d-135">isInline</span><span class="sxs-lookup"><span data-stu-id="c011d-135">isInline</span></span>|<span data-ttu-id="c011d-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="c011d-136">Boolean</span></span>|<span data-ttu-id="c011d-137">Defina como verdadeiro se o anexo é exibido embutido no corpo do objeto de incorporação.</span><span class="sxs-lookup"><span data-stu-id="c011d-137">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="c011d-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c011d-138">Optional.</span></span>|
|<span data-ttu-id="c011d-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c011d-139">lastModifiedDateTime</span></span>|<span data-ttu-id="c011d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c011d-140">DateTimeOffset</span></span>|<span data-ttu-id="c011d-141">Data e hora em que o anexo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c011d-141">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="c011d-142">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="c011d-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c011d-143">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c011d-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="c011d-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c011d-144">Optional.</span></span>|
|<span data-ttu-id="c011d-145">name</span><span class="sxs-lookup"><span data-stu-id="c011d-145">name</span></span>|<span data-ttu-id="c011d-146">String</span><span class="sxs-lookup"><span data-stu-id="c011d-146">String</span></span>|<span data-ttu-id="c011d-147">O texto que é exibido abaixo do ícone que representa o anexo incorporado.</span><span class="sxs-lookup"><span data-stu-id="c011d-147">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="c011d-148">Isso não precisa ser o nome de arquivo real.</span><span class="sxs-lookup"><span data-stu-id="c011d-148">This does not need to be the actual file name.</span></span> <span data-ttu-id="c011d-149">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c011d-149">Required.</span></span>|
|<span data-ttu-id="c011d-150">permissão</span><span class="sxs-lookup"><span data-stu-id="c011d-150">permission</span></span>|<span data-ttu-id="c011d-151">ReferenceAttachmentPermissions</span><span class="sxs-lookup"><span data-stu-id="c011d-151">ReferenceAttachmentPermissions</span></span>|<span data-ttu-id="c011d-152">Especifica as permissões concedidas pelo tipo de provedor na **providerType**o anexo.</span><span class="sxs-lookup"><span data-stu-id="c011d-152">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="c011d-153">Os valores possíveis são: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span><span class="sxs-lookup"><span data-stu-id="c011d-153">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="c011d-154">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c011d-154">Optional.</span></span>|
|<span data-ttu-id="c011d-155">previewUrl</span><span class="sxs-lookup"><span data-stu-id="c011d-155">previewUrl</span></span>|<span data-ttu-id="c011d-156">String</span><span class="sxs-lookup"><span data-stu-id="c011d-156">String</span></span>|<span data-ttu-id="c011d-157">Se aplica a apenas um anexo de referência de uma imagem - URL para obter uma imagem de visualização.</span><span class="sxs-lookup"><span data-stu-id="c011d-157">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="c011d-158">Use **thumbnailUrl** e **previewUrl** somente quando **sourceUrl** identifica um arquivo de imagem.</span><span class="sxs-lookup"><span data-stu-id="c011d-158">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="c011d-159">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c011d-159">Optional.</span></span>|
|<span data-ttu-id="c011d-160">providerType</span><span class="sxs-lookup"><span data-stu-id="c011d-160">providerType</span></span>|<span data-ttu-id="c011d-161">ReferenceAttachmentProviders</span><span class="sxs-lookup"><span data-stu-id="c011d-161">ReferenceAttachmentProviders</span></span>|<span data-ttu-id="c011d-162">O tipo de provedor que ofereça suporte a um anexo deste contentType.</span><span class="sxs-lookup"><span data-stu-id="c011d-162">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="c011d-163">Os valores possíveis são: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span><span class="sxs-lookup"><span data-stu-id="c011d-163">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="c011d-164">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c011d-164">Optional.</span></span>|
|<span data-ttu-id="c011d-165">size</span><span class="sxs-lookup"><span data-stu-id="c011d-165">size</span></span>|<span data-ttu-id="c011d-166">Int32</span><span class="sxs-lookup"><span data-stu-id="c011d-166">Int32</span></span>|<span data-ttu-id="c011d-167">O tamanho dos metadados em bytes que é armazenado na mensagem do anexo da referência.</span><span class="sxs-lookup"><span data-stu-id="c011d-167">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="c011d-168">Esse valor não indica o tamanho real do arquivo.</span><span class="sxs-lookup"><span data-stu-id="c011d-168">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="c011d-169">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c011d-169">Optional.</span></span>|
|<span data-ttu-id="c011d-170">Urlorigem</span><span class="sxs-lookup"><span data-stu-id="c011d-170">sourceUrl</span></span>|<span data-ttu-id="c011d-171">String</span><span class="sxs-lookup"><span data-stu-id="c011d-171">String</span></span>|<span data-ttu-id="c011d-172">URL para obter o conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="c011d-172">URL to get the attachment content.</span></span> <span data-ttu-id="c011d-173">Se essa for uma URL para uma pasta, em seguida, para a pasta para serem exibidos corretamente no Outlook ou no Outlook na web, defina **isFolder** como true.</span><span class="sxs-lookup"><span data-stu-id="c011d-173">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="c011d-174">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c011d-174">Required.</span></span>|
|<span data-ttu-id="c011d-175">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="c011d-175">thumbnailUrl</span></span>|<span data-ttu-id="c011d-176">String</span><span class="sxs-lookup"><span data-stu-id="c011d-176">String</span></span>|<span data-ttu-id="c011d-177">Se aplica a apenas um anexo de referência de uma imagem - URL para obter uma imagem em miniatura.</span><span class="sxs-lookup"><span data-stu-id="c011d-177">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="c011d-178">Use **thumbnailUrl** e **previewUrl** somente quando **sourceUrl** identifica um arquivo de imagem.</span><span class="sxs-lookup"><span data-stu-id="c011d-178">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="c011d-179">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c011d-179">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c011d-180">Relações</span><span class="sxs-lookup"><span data-stu-id="c011d-180">Relationships</span></span>
<span data-ttu-id="c011d-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c011d-181">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="c011d-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c011d-182">JSON representation</span></span>

<span data-ttu-id="c011d-183">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c011d-183">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
