---
title: Criar windowsPhone81AppX
description: Criar um novo objeto windowsPhone81AppX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 369658426555e682a832adfc3bdfdc3558edc95b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36322489"
---
# <a name="create-windowsphone81appx"></a><span data-ttu-id="ca8ad-103">Criar windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="ca8ad-103">Create windowsPhone81AppX</span></span>

> <span data-ttu-id="ca8ad-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca8ad-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca8ad-106">Criar um novo objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="ca8ad-106">Create a new [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca8ad-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ca8ad-107">Prerequisites</span></span>
<span data-ttu-id="ca8ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca8ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca8ad-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca8ad-110">Permission type</span></span>|<span data-ttu-id="ca8ad-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca8ad-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca8ad-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca8ad-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ca8ad-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca8ad-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-115">Not supported.</span></span>|
|<span data-ttu-id="ca8ad-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca8ad-116">Application</span></span>|<span data-ttu-id="ca8ad-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca8ad-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca8ad-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca8ad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ca8ad-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca8ad-119">Request headers</span></span>
|<span data-ttu-id="ca8ad-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca8ad-120">Header</span></span>|<span data-ttu-id="ca8ad-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ca8ad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca8ad-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca8ad-122">Authorization</span></span>|<span data-ttu-id="ca8ad-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca8ad-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ca8ad-124">Accept</span></span>|<span data-ttu-id="ca8ad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ca8ad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca8ad-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca8ad-126">Request body</span></span>
<span data-ttu-id="ca8ad-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81AppX.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-127">In the request body, supply a JSON representation for the windowsPhone81AppX object.</span></span>

<span data-ttu-id="ca8ad-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81AppX.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-128">The following table shows the properties that are required when you create the windowsPhone81AppX.</span></span>

|<span data-ttu-id="ca8ad-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca8ad-129">Property</span></span>|<span data-ttu-id="ca8ad-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca8ad-130">Type</span></span>|<span data-ttu-id="ca8ad-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca8ad-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca8ad-132">id</span><span class="sxs-lookup"><span data-stu-id="ca8ad-132">id</span></span>|<span data-ttu-id="ca8ad-133">String</span><span class="sxs-lookup"><span data-stu-id="ca8ad-133">String</span></span>|<span data-ttu-id="ca8ad-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-134">Key of the entity.</span></span> <span data-ttu-id="ca8ad-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ca8ad-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ca8ad-136">displayName</span></span>|<span data-ttu-id="ca8ad-137">String</span><span class="sxs-lookup"><span data-stu-id="ca8ad-137">String</span></span>|<span data-ttu-id="ca8ad-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ca8ad-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ca8ad-140">descrição</span><span class="sxs-lookup"><span data-stu-id="ca8ad-140">description</span></span>|<span data-ttu-id="ca8ad-141">String</span><span class="sxs-lookup"><span data-stu-id="ca8ad-141">String</span></span>|<span data-ttu-id="ca8ad-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-142">The description of the app.</span></span> <span data-ttu-id="ca8ad-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ca8ad-144">publicador</span><span class="sxs-lookup"><span data-stu-id="ca8ad-144">publisher</span></span>|<span data-ttu-id="ca8ad-145">String</span><span class="sxs-lookup"><span data-stu-id="ca8ad-145">String</span></span>|<span data-ttu-id="ca8ad-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-146">The publisher of the app.</span></span> <span data-ttu-id="ca8ad-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ca8ad-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ca8ad-148">largeIcon</span></span>|[<span data-ttu-id="ca8ad-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ca8ad-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ca8ad-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ca8ad-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ca8ad-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ca8ad-152">createdDateTime</span></span>|<span data-ttu-id="ca8ad-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca8ad-153">DateTimeOffset</span></span>|<span data-ttu-id="ca8ad-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-154">The date and time the app was created.</span></span> <span data-ttu-id="ca8ad-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ca8ad-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca8ad-156">lastModifiedDateTime</span></span>|<span data-ttu-id="ca8ad-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca8ad-157">DateTimeOffset</span></span>|<span data-ttu-id="ca8ad-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-158">The date and time the app was last modified.</span></span> <span data-ttu-id="ca8ad-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ca8ad-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ca8ad-160">isFeatured</span></span>|<span data-ttu-id="ca8ad-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca8ad-161">Boolean</span></span>|<span data-ttu-id="ca8ad-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ca8ad-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ca8ad-163">privacyInformationUrl</span></span>|<span data-ttu-id="ca8ad-164">String</span><span class="sxs-lookup"><span data-stu-id="ca8ad-164">String</span></span>|<span data-ttu-id="ca8ad-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-165">The privacy statement Url.</span></span> <span data-ttu-id="ca8ad-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ca8ad-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ca8ad-167">informationUrl</span></span>|<span data-ttu-id="ca8ad-168">String</span><span class="sxs-lookup"><span data-stu-id="ca8ad-168">String</span></span>|<span data-ttu-id="ca8ad-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-169">The more information Url.</span></span> <span data-ttu-id="ca8ad-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ca8ad-171">owner</span><span class="sxs-lookup"><span data-stu-id="ca8ad-171">owner</span></span>|<span data-ttu-id="ca8ad-172">String</span><span class="sxs-lookup"><span data-stu-id="ca8ad-172">String</span></span>|<span data-ttu-id="ca8ad-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-173">The owner of the app.</span></span> <span data-ttu-id="ca8ad-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ca8ad-175">developer</span><span class="sxs-lookup"><span data-stu-id="ca8ad-175">developer</span></span>|<span data-ttu-id="ca8ad-176">String</span><span class="sxs-lookup"><span data-stu-id="ca8ad-176">String</span></span>|<span data-ttu-id="ca8ad-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-177">The developer of the app.</span></span> <span data-ttu-id="ca8ad-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ca8ad-179">notes</span><span class="sxs-lookup"><span data-stu-id="ca8ad-179">notes</span></span>|<span data-ttu-id="ca8ad-180">String</span><span class="sxs-lookup"><span data-stu-id="ca8ad-180">String</span></span>|<span data-ttu-id="ca8ad-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-181">Notes for the app.</span></span> <span data-ttu-id="ca8ad-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ca8ad-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="ca8ad-183">uploadState</span></span>|<span data-ttu-id="ca8ad-184">Int32</span><span class="sxs-lookup"><span data-stu-id="ca8ad-184">Int32</span></span>|<span data-ttu-id="ca8ad-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-185">The upload state.</span></span> <span data-ttu-id="ca8ad-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ca8ad-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="ca8ad-187">publishingState</span></span>|[<span data-ttu-id="ca8ad-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ca8ad-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ca8ad-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-189">The publishing state for the app.</span></span> <span data-ttu-id="ca8ad-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ca8ad-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ca8ad-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="ca8ad-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ca8ad-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ca8ad-193">isAssigned</span></span>|<span data-ttu-id="ca8ad-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca8ad-194">Boolean</span></span>|<span data-ttu-id="ca8ad-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ca8ad-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ca8ad-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ca8ad-197">roleScopeTagIds</span></span>|<span data-ttu-id="ca8ad-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca8ad-198">String collection</span></span>|<span data-ttu-id="ca8ad-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ca8ad-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ca8ad-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="ca8ad-201">dependentAppCount</span></span>|<span data-ttu-id="ca8ad-202">Int32</span><span class="sxs-lookup"><span data-stu-id="ca8ad-202">Int32</span></span>|<span data-ttu-id="ca8ad-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="ca8ad-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ca8ad-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ca8ad-205">committedContentVersion</span></span>|<span data-ttu-id="ca8ad-206">String</span><span class="sxs-lookup"><span data-stu-id="ca8ad-206">String</span></span>|<span data-ttu-id="ca8ad-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-207">The internal committed content version.</span></span> <span data-ttu-id="ca8ad-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ca8ad-209">fileName</span><span class="sxs-lookup"><span data-stu-id="ca8ad-209">fileName</span></span>|<span data-ttu-id="ca8ad-210">String</span><span class="sxs-lookup"><span data-stu-id="ca8ad-210">String</span></span>|<span data-ttu-id="ca8ad-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-211">The name of the main Lob application file.</span></span> <span data-ttu-id="ca8ad-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ca8ad-213">size</span><span class="sxs-lookup"><span data-stu-id="ca8ad-213">size</span></span>|<span data-ttu-id="ca8ad-214">Int64</span><span class="sxs-lookup"><span data-stu-id="ca8ad-214">Int64</span></span>|<span data-ttu-id="ca8ad-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="ca8ad-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca8ad-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ca8ad-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="ca8ad-217">applicableArchitectures</span></span>|[<span data-ttu-id="ca8ad-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="ca8ad-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="ca8ad-219">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="ca8ad-220">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="ca8ad-221">identityName</span><span class="sxs-lookup"><span data-stu-id="ca8ad-221">identityName</span></span>|<span data-ttu-id="ca8ad-222">String</span><span class="sxs-lookup"><span data-stu-id="ca8ad-222">String</span></span>|<span data-ttu-id="ca8ad-223">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-223">The Identity Name.</span></span>|
|<span data-ttu-id="ca8ad-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="ca8ad-224">identityPublisherHash</span></span>|<span data-ttu-id="ca8ad-225">String</span><span class="sxs-lookup"><span data-stu-id="ca8ad-225">String</span></span>|<span data-ttu-id="ca8ad-226">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="ca8ad-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="ca8ad-227">identityResourceIdentifier</span></span>|<span data-ttu-id="ca8ad-228">String</span><span class="sxs-lookup"><span data-stu-id="ca8ad-228">String</span></span>|<span data-ttu-id="ca8ad-229">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="ca8ad-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ca8ad-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ca8ad-231">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ca8ad-231">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="ca8ad-232">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-232">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ca8ad-233">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="ca8ad-233">phoneProductIdentifier</span></span>|<span data-ttu-id="ca8ad-234">String</span><span class="sxs-lookup"><span data-stu-id="ca8ad-234">String</span></span>|<span data-ttu-id="ca8ad-235">O identificador do produto de telefone.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-235">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="ca8ad-236">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="ca8ad-236">phonePublisherId</span></span>|<span data-ttu-id="ca8ad-237">String</span><span class="sxs-lookup"><span data-stu-id="ca8ad-237">String</span></span>|<span data-ttu-id="ca8ad-238">A ID do editor do telefone.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-238">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="ca8ad-239">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ca8ad-239">identityVersion</span></span>|<span data-ttu-id="ca8ad-240">String</span><span class="sxs-lookup"><span data-stu-id="ca8ad-240">String</span></span>|<span data-ttu-id="ca8ad-241">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-241">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="ca8ad-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca8ad-242">Response</span></span>
<span data-ttu-id="ca8ad-243">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-243">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca8ad-244">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca8ad-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca8ad-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca8ad-245">Request</span></span>
<span data-ttu-id="ca8ad-246">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-246">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1513

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
  "dependentAppCount": 1,
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
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="ca8ad-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca8ad-247">Response</span></span>
<span data-ttu-id="ca8ad-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca8ad-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1685

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
  "dependentAppCount": 1,
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
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```






