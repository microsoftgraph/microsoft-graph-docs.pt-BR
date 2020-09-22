---
title: Criar windowsUniversalAppX
description: Cria um novo objeto windowsUniversalAppX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e9da3ba80ffb56efe1f0f303dcec59040a3e5c25
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063489"
---
# <a name="create-windowsuniversalappx"></a><span data-ttu-id="27020-103">Criar windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="27020-103">Create windowsUniversalAppX</span></span>

<span data-ttu-id="27020-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27020-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27020-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="27020-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27020-106">Cria um novo objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="27020-106">Create a new [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27020-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="27020-107">Prerequisites</span></span>
<span data-ttu-id="27020-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27020-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27020-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27020-110">Permission type</span></span>|<span data-ttu-id="27020-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="27020-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27020-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27020-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27020-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27020-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="27020-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27020-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27020-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27020-115">Not supported.</span></span>|
|<span data-ttu-id="27020-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27020-116">Application</span></span>|<span data-ttu-id="27020-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27020-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27020-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27020-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="27020-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27020-119">Request headers</span></span>
|<span data-ttu-id="27020-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27020-120">Header</span></span>|<span data-ttu-id="27020-121">Valor</span><span class="sxs-lookup"><span data-stu-id="27020-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27020-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="27020-122">Authorization</span></span>|<span data-ttu-id="27020-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27020-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27020-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="27020-124">Accept</span></span>|<span data-ttu-id="27020-125">application/json</span><span class="sxs-lookup"><span data-stu-id="27020-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27020-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27020-126">Request body</span></span>
<span data-ttu-id="27020-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="27020-127">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="27020-128">A tabela a seguir mostra as propriedades obrigatórias ao criar windowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="27020-128">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="27020-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27020-129">Property</span></span>|<span data-ttu-id="27020-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="27020-130">Type</span></span>|<span data-ttu-id="27020-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="27020-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27020-132">id</span><span class="sxs-lookup"><span data-stu-id="27020-132">id</span></span>|<span data-ttu-id="27020-133">String</span><span class="sxs-lookup"><span data-stu-id="27020-133">String</span></span>|<span data-ttu-id="27020-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="27020-134">Key of the entity.</span></span> <span data-ttu-id="27020-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27020-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27020-136">displayName</span><span class="sxs-lookup"><span data-stu-id="27020-136">displayName</span></span>|<span data-ttu-id="27020-137">String</span><span class="sxs-lookup"><span data-stu-id="27020-137">String</span></span>|<span data-ttu-id="27020-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="27020-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="27020-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27020-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27020-140">description</span><span class="sxs-lookup"><span data-stu-id="27020-140">description</span></span>|<span data-ttu-id="27020-141">String</span><span class="sxs-lookup"><span data-stu-id="27020-141">String</span></span>|<span data-ttu-id="27020-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="27020-142">The description of the app.</span></span> <span data-ttu-id="27020-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27020-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27020-144">publicador</span><span class="sxs-lookup"><span data-stu-id="27020-144">publisher</span></span>|<span data-ttu-id="27020-145">String</span><span class="sxs-lookup"><span data-stu-id="27020-145">String</span></span>|<span data-ttu-id="27020-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="27020-146">The publisher of the app.</span></span> <span data-ttu-id="27020-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27020-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27020-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="27020-148">largeIcon</span></span>|[<span data-ttu-id="27020-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="27020-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="27020-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="27020-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="27020-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27020-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27020-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27020-152">createdDateTime</span></span>|<span data-ttu-id="27020-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27020-153">DateTimeOffset</span></span>|<span data-ttu-id="27020-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="27020-154">The date and time the app was created.</span></span> <span data-ttu-id="27020-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27020-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27020-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27020-156">lastModifiedDateTime</span></span>|<span data-ttu-id="27020-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27020-157">DateTimeOffset</span></span>|<span data-ttu-id="27020-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="27020-158">The date and time the app was last modified.</span></span> <span data-ttu-id="27020-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27020-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27020-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="27020-160">isFeatured</span></span>|<span data-ttu-id="27020-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="27020-161">Boolean</span></span>|<span data-ttu-id="27020-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27020-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27020-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="27020-163">privacyInformationUrl</span></span>|<span data-ttu-id="27020-164">String</span><span class="sxs-lookup"><span data-stu-id="27020-164">String</span></span>|<span data-ttu-id="27020-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="27020-165">The privacy statement Url.</span></span> <span data-ttu-id="27020-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27020-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27020-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="27020-167">informationUrl</span></span>|<span data-ttu-id="27020-168">String</span><span class="sxs-lookup"><span data-stu-id="27020-168">String</span></span>|<span data-ttu-id="27020-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="27020-169">The more information Url.</span></span> <span data-ttu-id="27020-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27020-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27020-171">proprietário</span><span class="sxs-lookup"><span data-stu-id="27020-171">owner</span></span>|<span data-ttu-id="27020-172">String</span><span class="sxs-lookup"><span data-stu-id="27020-172">String</span></span>|<span data-ttu-id="27020-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="27020-173">The owner of the app.</span></span> <span data-ttu-id="27020-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27020-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27020-175">developer</span><span class="sxs-lookup"><span data-stu-id="27020-175">developer</span></span>|<span data-ttu-id="27020-176">String</span><span class="sxs-lookup"><span data-stu-id="27020-176">String</span></span>|<span data-ttu-id="27020-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="27020-177">The developer of the app.</span></span> <span data-ttu-id="27020-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27020-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27020-179">notes</span><span class="sxs-lookup"><span data-stu-id="27020-179">notes</span></span>|<span data-ttu-id="27020-180">String</span><span class="sxs-lookup"><span data-stu-id="27020-180">String</span></span>|<span data-ttu-id="27020-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="27020-181">Notes for the app.</span></span> <span data-ttu-id="27020-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="27020-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27020-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="27020-183">publishingState</span></span>|[<span data-ttu-id="27020-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="27020-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="27020-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="27020-185">The publishing state for the app.</span></span> <span data-ttu-id="27020-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="27020-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="27020-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="27020-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="27020-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="27020-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="27020-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="27020-189">committedContentVersion</span></span>|<span data-ttu-id="27020-190">String</span><span class="sxs-lookup"><span data-stu-id="27020-190">String</span></span>|<span data-ttu-id="27020-191">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="27020-191">The internal committed content version.</span></span> <span data-ttu-id="27020-192">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="27020-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="27020-193">fileName</span><span class="sxs-lookup"><span data-stu-id="27020-193">fileName</span></span>|<span data-ttu-id="27020-194">String</span><span class="sxs-lookup"><span data-stu-id="27020-194">String</span></span>|<span data-ttu-id="27020-195">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="27020-195">The name of the main Lob application file.</span></span> <span data-ttu-id="27020-196">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="27020-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="27020-197">size</span><span class="sxs-lookup"><span data-stu-id="27020-197">size</span></span>|<span data-ttu-id="27020-198">Int64</span><span class="sxs-lookup"><span data-stu-id="27020-198">Int64</span></span>|<span data-ttu-id="27020-199">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="27020-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="27020-200">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="27020-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="27020-201">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="27020-201">applicableArchitectures</span></span>|[<span data-ttu-id="27020-202">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="27020-202">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="27020-203">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="27020-203">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="27020-204">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="27020-204">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="27020-205">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="27020-205">applicableDeviceTypes</span></span>|[<span data-ttu-id="27020-206">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="27020-206">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="27020-207">Os tipos de dispositivos Windows nos quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="27020-207">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="27020-208">Os valores possíveis são: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="27020-208">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="27020-209">identityName</span><span class="sxs-lookup"><span data-stu-id="27020-209">identityName</span></span>|<span data-ttu-id="27020-210">String</span><span class="sxs-lookup"><span data-stu-id="27020-210">String</span></span>|<span data-ttu-id="27020-211">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="27020-211">The Identity Name.</span></span>|
|<span data-ttu-id="27020-212">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="27020-212">identityPublisherHash</span></span>|<span data-ttu-id="27020-213">String</span><span class="sxs-lookup"><span data-stu-id="27020-213">String</span></span>|<span data-ttu-id="27020-214">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="27020-214">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="27020-215">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="27020-215">identityResourceIdentifier</span></span>|<span data-ttu-id="27020-216">String</span><span class="sxs-lookup"><span data-stu-id="27020-216">String</span></span>|<span data-ttu-id="27020-217">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="27020-217">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="27020-218">isBundle</span><span class="sxs-lookup"><span data-stu-id="27020-218">isBundle</span></span>|<span data-ttu-id="27020-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="27020-219">Boolean</span></span>|<span data-ttu-id="27020-220">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="27020-220">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="27020-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="27020-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="27020-222">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="27020-222">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="27020-223">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="27020-223">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="27020-224">identityVersion</span><span class="sxs-lookup"><span data-stu-id="27020-224">identityVersion</span></span>|<span data-ttu-id="27020-225">String</span><span class="sxs-lookup"><span data-stu-id="27020-225">String</span></span>|<span data-ttu-id="27020-226">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="27020-226">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="27020-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="27020-227">Response</span></span>
<span data-ttu-id="27020-228">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27020-228">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27020-229">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27020-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="27020-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27020-230">Request</span></span>
<span data-ttu-id="27020-231">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27020-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1189

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="27020-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="27020-232">Response</span></span>
<span data-ttu-id="27020-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27020-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```









