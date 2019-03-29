---
title: Criar windowsPhone81AppX
description: Criar um novo objeto windowsPhone81AppX.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5aa592c91c6680a1b0872c203a10b1a3f4eec55f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983166"
---
# <a name="create-windowsphone81appx"></a><span data-ttu-id="11c09-103">Criar windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="11c09-103">Create windowsPhone81AppX</span></span>

> <span data-ttu-id="11c09-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="11c09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11c09-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="11c09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11c09-106">Criar um novo objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="11c09-106">Create a new [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11c09-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="11c09-107">Prerequisites</span></span>
<span data-ttu-id="11c09-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11c09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11c09-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11c09-110">Permission type</span></span>|<span data-ttu-id="11c09-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="11c09-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11c09-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11c09-112">Delegated (work or school account)</span></span>|<span data-ttu-id="11c09-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11c09-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="11c09-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11c09-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11c09-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11c09-115">Not supported.</span></span>|
|<span data-ttu-id="11c09-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11c09-116">Application</span></span>|<span data-ttu-id="11c09-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11c09-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11c09-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11c09-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="11c09-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11c09-119">Request headers</span></span>
|<span data-ttu-id="11c09-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="11c09-120">Header</span></span>|<span data-ttu-id="11c09-121">Valor</span><span class="sxs-lookup"><span data-stu-id="11c09-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11c09-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="11c09-122">Authorization</span></span>|<span data-ttu-id="11c09-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11c09-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11c09-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="11c09-124">Accept</span></span>|<span data-ttu-id="11c09-125">application/json</span><span class="sxs-lookup"><span data-stu-id="11c09-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11c09-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11c09-126">Request body</span></span>
<span data-ttu-id="11c09-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81AppX.</span><span class="sxs-lookup"><span data-stu-id="11c09-127">In the request body, supply a JSON representation for the windowsPhone81AppX object.</span></span>

<span data-ttu-id="11c09-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81AppX.</span><span class="sxs-lookup"><span data-stu-id="11c09-128">The following table shows the properties that are required when you create the windowsPhone81AppX.</span></span>

|<span data-ttu-id="11c09-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11c09-129">Property</span></span>|<span data-ttu-id="11c09-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="11c09-130">Type</span></span>|<span data-ttu-id="11c09-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="11c09-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11c09-132">id</span><span class="sxs-lookup"><span data-stu-id="11c09-132">id</span></span>|<span data-ttu-id="11c09-133">String</span><span class="sxs-lookup"><span data-stu-id="11c09-133">String</span></span>|<span data-ttu-id="11c09-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="11c09-134">Key of the entity.</span></span> <span data-ttu-id="11c09-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11c09-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11c09-136">displayName</span><span class="sxs-lookup"><span data-stu-id="11c09-136">displayName</span></span>|<span data-ttu-id="11c09-137">String</span><span class="sxs-lookup"><span data-stu-id="11c09-137">String</span></span>|<span data-ttu-id="11c09-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="11c09-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="11c09-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11c09-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11c09-140">descrição</span><span class="sxs-lookup"><span data-stu-id="11c09-140">description</span></span>|<span data-ttu-id="11c09-141">String</span><span class="sxs-lookup"><span data-stu-id="11c09-141">String</span></span>|<span data-ttu-id="11c09-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11c09-142">The description of the app.</span></span> <span data-ttu-id="11c09-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11c09-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11c09-144">publicador</span><span class="sxs-lookup"><span data-stu-id="11c09-144">publisher</span></span>|<span data-ttu-id="11c09-145">String</span><span class="sxs-lookup"><span data-stu-id="11c09-145">String</span></span>|<span data-ttu-id="11c09-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11c09-146">The publisher of the app.</span></span> <span data-ttu-id="11c09-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11c09-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11c09-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="11c09-148">largeIcon</span></span>|[<span data-ttu-id="11c09-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="11c09-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="11c09-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="11c09-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="11c09-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11c09-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11c09-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11c09-152">createdDateTime</span></span>|<span data-ttu-id="11c09-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11c09-153">DateTimeOffset</span></span>|<span data-ttu-id="11c09-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11c09-154">The date and time the app was created.</span></span> <span data-ttu-id="11c09-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11c09-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11c09-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11c09-156">lastModifiedDateTime</span></span>|<span data-ttu-id="11c09-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11c09-157">DateTimeOffset</span></span>|<span data-ttu-id="11c09-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="11c09-158">The date and time the app was last modified.</span></span> <span data-ttu-id="11c09-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11c09-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11c09-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="11c09-160">isFeatured</span></span>|<span data-ttu-id="11c09-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="11c09-161">Boolean</span></span>|<span data-ttu-id="11c09-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11c09-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11c09-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="11c09-163">privacyInformationUrl</span></span>|<span data-ttu-id="11c09-164">String</span><span class="sxs-lookup"><span data-stu-id="11c09-164">String</span></span>|<span data-ttu-id="11c09-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="11c09-165">The privacy statement Url.</span></span> <span data-ttu-id="11c09-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11c09-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11c09-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="11c09-167">informationUrl</span></span>|<span data-ttu-id="11c09-168">String</span><span class="sxs-lookup"><span data-stu-id="11c09-168">String</span></span>|<span data-ttu-id="11c09-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="11c09-169">The more information Url.</span></span> <span data-ttu-id="11c09-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11c09-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11c09-171">owner</span><span class="sxs-lookup"><span data-stu-id="11c09-171">owner</span></span>|<span data-ttu-id="11c09-172">String</span><span class="sxs-lookup"><span data-stu-id="11c09-172">String</span></span>|<span data-ttu-id="11c09-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="11c09-173">The owner of the app.</span></span> <span data-ttu-id="11c09-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11c09-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11c09-175">developer</span><span class="sxs-lookup"><span data-stu-id="11c09-175">developer</span></span>|<span data-ttu-id="11c09-176">String</span><span class="sxs-lookup"><span data-stu-id="11c09-176">String</span></span>|<span data-ttu-id="11c09-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11c09-177">The developer of the app.</span></span> <span data-ttu-id="11c09-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11c09-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11c09-179">notes</span><span class="sxs-lookup"><span data-stu-id="11c09-179">notes</span></span>|<span data-ttu-id="11c09-180">String</span><span class="sxs-lookup"><span data-stu-id="11c09-180">String</span></span>|<span data-ttu-id="11c09-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11c09-181">Notes for the app.</span></span> <span data-ttu-id="11c09-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11c09-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11c09-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="11c09-183">uploadState</span></span>|<span data-ttu-id="11c09-184">Int32</span><span class="sxs-lookup"><span data-stu-id="11c09-184">Int32</span></span>|<span data-ttu-id="11c09-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="11c09-185">The upload state.</span></span> <span data-ttu-id="11c09-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11c09-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11c09-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="11c09-187">publishingState</span></span>|[<span data-ttu-id="11c09-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="11c09-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="11c09-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11c09-189">The publishing state for the app.</span></span> <span data-ttu-id="11c09-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="11c09-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="11c09-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="11c09-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="11c09-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="11c09-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="11c09-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="11c09-193">isAssigned</span></span>|<span data-ttu-id="11c09-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="11c09-194">Boolean</span></span>|<span data-ttu-id="11c09-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="11c09-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="11c09-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11c09-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11c09-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="11c09-197">roleScopeTagIds</span></span>|<span data-ttu-id="11c09-198">Coleção String</span><span class="sxs-lookup"><span data-stu-id="11c09-198">String collection</span></span>|<span data-ttu-id="11c09-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="11c09-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="11c09-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11c09-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11c09-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="11c09-201">committedContentVersion</span></span>|<span data-ttu-id="11c09-202">String</span><span class="sxs-lookup"><span data-stu-id="11c09-202">String</span></span>|<span data-ttu-id="11c09-203">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="11c09-203">The internal committed content version.</span></span> <span data-ttu-id="11c09-204">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="11c09-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="11c09-205">fileName</span><span class="sxs-lookup"><span data-stu-id="11c09-205">fileName</span></span>|<span data-ttu-id="11c09-206">String</span><span class="sxs-lookup"><span data-stu-id="11c09-206">String</span></span>|<span data-ttu-id="11c09-207">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="11c09-207">The name of the main Lob application file.</span></span> <span data-ttu-id="11c09-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="11c09-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="11c09-209">size</span><span class="sxs-lookup"><span data-stu-id="11c09-209">size</span></span>|<span data-ttu-id="11c09-210">Int64</span><span class="sxs-lookup"><span data-stu-id="11c09-210">Int64</span></span>|<span data-ttu-id="11c09-211">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="11c09-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="11c09-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="11c09-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="11c09-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="11c09-213">applicableArchitectures</span></span>|[<span data-ttu-id="11c09-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="11c09-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="11c09-215">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="11c09-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="11c09-216">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="11c09-216">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="11c09-217">identityName</span><span class="sxs-lookup"><span data-stu-id="11c09-217">identityName</span></span>|<span data-ttu-id="11c09-218">String</span><span class="sxs-lookup"><span data-stu-id="11c09-218">String</span></span>|<span data-ttu-id="11c09-219">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="11c09-219">The Identity Name.</span></span>|
|<span data-ttu-id="11c09-220">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="11c09-220">identityPublisherHash</span></span>|<span data-ttu-id="11c09-221">String</span><span class="sxs-lookup"><span data-stu-id="11c09-221">String</span></span>|<span data-ttu-id="11c09-222">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="11c09-222">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="11c09-223">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="11c09-223">identityResourceIdentifier</span></span>|<span data-ttu-id="11c09-224">String</span><span class="sxs-lookup"><span data-stu-id="11c09-224">String</span></span>|<span data-ttu-id="11c09-225">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="11c09-225">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="11c09-226">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="11c09-226">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="11c09-227">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="11c09-227">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="11c09-228">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="11c09-228">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="11c09-229">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="11c09-229">phoneProductIdentifier</span></span>|<span data-ttu-id="11c09-230">String</span><span class="sxs-lookup"><span data-stu-id="11c09-230">String</span></span>|<span data-ttu-id="11c09-231">O identificador do produto de telefone.</span><span class="sxs-lookup"><span data-stu-id="11c09-231">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="11c09-232">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="11c09-232">phonePublisherId</span></span>|<span data-ttu-id="11c09-233">String</span><span class="sxs-lookup"><span data-stu-id="11c09-233">String</span></span>|<span data-ttu-id="11c09-234">A ID do editor do telefone.</span><span class="sxs-lookup"><span data-stu-id="11c09-234">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="11c09-235">identityVersion</span><span class="sxs-lookup"><span data-stu-id="11c09-235">identityVersion</span></span>|<span data-ttu-id="11c09-236">String</span><span class="sxs-lookup"><span data-stu-id="11c09-236">String</span></span>|<span data-ttu-id="11c09-237">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="11c09-237">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="11c09-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="11c09-238">Response</span></span>
<span data-ttu-id="11c09-239">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11c09-239">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11c09-240">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11c09-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="11c09-241">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11c09-241">Request</span></span>
<span data-ttu-id="11c09-242">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11c09-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1440

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="11c09-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="11c09-243">Response</span></span>
<span data-ttu-id="11c09-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11c09-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1612

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
  "id": "4ff27f80-7f80-4ff2-807f-f24f807ff24f",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```




