---
title: Criar windowsUniversalAppX
description: Cria um novo objeto windowsUniversalAppX.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5bdbab2d23d3777e72aa291a9729f0480793883f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149767"
---
# <a name="create-windowsuniversalappx"></a><span data-ttu-id="cc46b-103">Criar windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="cc46b-103">Create windowsUniversalAppX</span></span>

> <span data-ttu-id="cc46b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cc46b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc46b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cc46b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc46b-106">Cria um novo objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="cc46b-106">Create a new [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc46b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cc46b-107">Prerequisites</span></span>
<span data-ttu-id="cc46b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cc46b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cc46b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc46b-110">Permission type</span></span>|<span data-ttu-id="cc46b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cc46b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc46b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc46b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cc46b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc46b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cc46b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc46b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc46b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc46b-115">Not supported.</span></span>|
|<span data-ttu-id="cc46b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc46b-116">Application</span></span>|<span data-ttu-id="cc46b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc46b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc46b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc46b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="cc46b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc46b-119">Request headers</span></span>
|<span data-ttu-id="cc46b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cc46b-120">Header</span></span>|<span data-ttu-id="cc46b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cc46b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc46b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc46b-122">Authorization</span></span>|<span data-ttu-id="cc46b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc46b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc46b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cc46b-124">Accept</span></span>|<span data-ttu-id="cc46b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cc46b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc46b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc46b-126">Request body</span></span>
<span data-ttu-id="cc46b-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="cc46b-127">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="cc46b-128">A tabela a seguir mostra as propriedades obrigatórias ao criar windowsUniversalAppX.</span><span class="sxs-lookup"><span data-stu-id="cc46b-128">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="cc46b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc46b-129">Property</span></span>|<span data-ttu-id="cc46b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc46b-130">Type</span></span>|<span data-ttu-id="cc46b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc46b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc46b-132">id</span><span class="sxs-lookup"><span data-stu-id="cc46b-132">id</span></span>|<span data-ttu-id="cc46b-133">String</span><span class="sxs-lookup"><span data-stu-id="cc46b-133">String</span></span>|<span data-ttu-id="cc46b-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cc46b-134">Key of the entity.</span></span> <span data-ttu-id="cc46b-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cc46b-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc46b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cc46b-136">displayName</span></span>|<span data-ttu-id="cc46b-137">String</span><span class="sxs-lookup"><span data-stu-id="cc46b-137">String</span></span>|<span data-ttu-id="cc46b-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="cc46b-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cc46b-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cc46b-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc46b-140">description</span><span class="sxs-lookup"><span data-stu-id="cc46b-140">description</span></span>|<span data-ttu-id="cc46b-141">String</span><span class="sxs-lookup"><span data-stu-id="cc46b-141">String</span></span>|<span data-ttu-id="cc46b-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cc46b-142">The description of the app.</span></span> <span data-ttu-id="cc46b-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cc46b-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc46b-144">publisher</span><span class="sxs-lookup"><span data-stu-id="cc46b-144">publisher</span></span>|<span data-ttu-id="cc46b-145">String</span><span class="sxs-lookup"><span data-stu-id="cc46b-145">String</span></span>|<span data-ttu-id="cc46b-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cc46b-146">The publisher of the app.</span></span> <span data-ttu-id="cc46b-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cc46b-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc46b-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cc46b-148">largeIcon</span></span>|[<span data-ttu-id="cc46b-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cc46b-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cc46b-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="cc46b-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cc46b-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cc46b-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc46b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc46b-152">createdDateTime</span></span>|<span data-ttu-id="cc46b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc46b-153">DateTimeOffset</span></span>|<span data-ttu-id="cc46b-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cc46b-154">The date and time the app was created.</span></span> <span data-ttu-id="cc46b-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cc46b-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc46b-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc46b-156">lastModifiedDateTime</span></span>|<span data-ttu-id="cc46b-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc46b-157">DateTimeOffset</span></span>|<span data-ttu-id="cc46b-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="cc46b-158">The date and time the app was last modified.</span></span> <span data-ttu-id="cc46b-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cc46b-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc46b-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cc46b-160">isFeatured</span></span>|<span data-ttu-id="cc46b-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc46b-161">Boolean</span></span>|<span data-ttu-id="cc46b-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cc46b-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc46b-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cc46b-163">privacyInformationUrl</span></span>|<span data-ttu-id="cc46b-164">String</span><span class="sxs-lookup"><span data-stu-id="cc46b-164">String</span></span>|<span data-ttu-id="cc46b-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="cc46b-165">The privacy statement Url.</span></span> <span data-ttu-id="cc46b-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cc46b-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc46b-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cc46b-167">informationUrl</span></span>|<span data-ttu-id="cc46b-168">String</span><span class="sxs-lookup"><span data-stu-id="cc46b-168">String</span></span>|<span data-ttu-id="cc46b-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="cc46b-169">The more information Url.</span></span> <span data-ttu-id="cc46b-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cc46b-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc46b-171">owner</span><span class="sxs-lookup"><span data-stu-id="cc46b-171">owner</span></span>|<span data-ttu-id="cc46b-172">String</span><span class="sxs-lookup"><span data-stu-id="cc46b-172">String</span></span>|<span data-ttu-id="cc46b-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="cc46b-173">The owner of the app.</span></span> <span data-ttu-id="cc46b-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cc46b-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc46b-175">developer</span><span class="sxs-lookup"><span data-stu-id="cc46b-175">developer</span></span>|<span data-ttu-id="cc46b-176">String</span><span class="sxs-lookup"><span data-stu-id="cc46b-176">String</span></span>|<span data-ttu-id="cc46b-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cc46b-177">The developer of the app.</span></span> <span data-ttu-id="cc46b-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cc46b-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc46b-179">Observações</span><span class="sxs-lookup"><span data-stu-id="cc46b-179">notes</span></span>|<span data-ttu-id="cc46b-180">String</span><span class="sxs-lookup"><span data-stu-id="cc46b-180">String</span></span>|<span data-ttu-id="cc46b-181">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cc46b-181">Notes for the app.</span></span> <span data-ttu-id="cc46b-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cc46b-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc46b-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="cc46b-183">uploadState</span></span>|<span data-ttu-id="cc46b-184">Int32</span><span class="sxs-lookup"><span data-stu-id="cc46b-184">Int32</span></span>|<span data-ttu-id="cc46b-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="cc46b-185">The upload state.</span></span> <span data-ttu-id="cc46b-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cc46b-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc46b-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="cc46b-187">publishingState</span></span>|[<span data-ttu-id="cc46b-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="cc46b-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="cc46b-189">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cc46b-189">The publishing state for the app.</span></span> <span data-ttu-id="cc46b-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="cc46b-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cc46b-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cc46b-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="cc46b-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="cc46b-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cc46b-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="cc46b-193">isAssigned</span></span>|<span data-ttu-id="cc46b-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc46b-194">Boolean</span></span>|<span data-ttu-id="cc46b-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="cc46b-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="cc46b-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cc46b-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc46b-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cc46b-197">roleScopeTagIds</span></span>|<span data-ttu-id="cc46b-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc46b-198">String collection</span></span>|<span data-ttu-id="cc46b-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="cc46b-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="cc46b-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cc46b-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cc46b-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="cc46b-201">committedContentVersion</span></span>|<span data-ttu-id="cc46b-202">String</span><span class="sxs-lookup"><span data-stu-id="cc46b-202">String</span></span>|<span data-ttu-id="cc46b-203">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="cc46b-203">The internal committed content version.</span></span> <span data-ttu-id="cc46b-204">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cc46b-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="cc46b-205">fileName</span><span class="sxs-lookup"><span data-stu-id="cc46b-205">fileName</span></span>|<span data-ttu-id="cc46b-206">String</span><span class="sxs-lookup"><span data-stu-id="cc46b-206">String</span></span>|<span data-ttu-id="cc46b-207">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="cc46b-207">The name of the main Lob application file.</span></span> <span data-ttu-id="cc46b-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cc46b-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="cc46b-209">size</span><span class="sxs-lookup"><span data-stu-id="cc46b-209">size</span></span>|<span data-ttu-id="cc46b-210">Int64</span><span class="sxs-lookup"><span data-stu-id="cc46b-210">Int64</span></span>|<span data-ttu-id="cc46b-211">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="cc46b-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="cc46b-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cc46b-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="cc46b-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="cc46b-213">applicableArchitectures</span></span>|[<span data-ttu-id="cc46b-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="cc46b-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="cc46b-215">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="cc46b-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="cc46b-216">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="cc46b-216">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="cc46b-217">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="cc46b-217">applicableDeviceTypes</span></span>|[<span data-ttu-id="cc46b-218">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="cc46b-218">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="cc46b-219">Os tipos de dispositivos Windows nos quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="cc46b-219">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="cc46b-220">Os valores possíveis são: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="cc46b-220">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="cc46b-221">identityName</span><span class="sxs-lookup"><span data-stu-id="cc46b-221">identityName</span></span>|<span data-ttu-id="cc46b-222">String</span><span class="sxs-lookup"><span data-stu-id="cc46b-222">String</span></span>|<span data-ttu-id="cc46b-223">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="cc46b-223">The Identity Name.</span></span>|
|<span data-ttu-id="cc46b-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="cc46b-224">identityPublisherHash</span></span>|<span data-ttu-id="cc46b-225">String</span><span class="sxs-lookup"><span data-stu-id="cc46b-225">String</span></span>|<span data-ttu-id="cc46b-226">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="cc46b-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="cc46b-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="cc46b-227">identityResourceIdentifier</span></span>|<span data-ttu-id="cc46b-228">String</span><span class="sxs-lookup"><span data-stu-id="cc46b-228">String</span></span>|<span data-ttu-id="cc46b-229">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="cc46b-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="cc46b-230">isBundle</span><span class="sxs-lookup"><span data-stu-id="cc46b-230">isBundle</span></span>|<span data-ttu-id="cc46b-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc46b-231">Boolean</span></span>|<span data-ttu-id="cc46b-232">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="cc46b-232">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="cc46b-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cc46b-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="cc46b-234">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cc46b-234">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="cc46b-235">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="cc46b-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="cc46b-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="cc46b-236">identityVersion</span></span>|<span data-ttu-id="cc46b-237">String</span><span class="sxs-lookup"><span data-stu-id="cc46b-237">String</span></span>|<span data-ttu-id="cc46b-238">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="cc46b-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="cc46b-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc46b-239">Response</span></span>
<span data-ttu-id="cc46b-240">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc46b-240">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc46b-241">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc46b-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc46b-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc46b-242">Request</span></span>
<span data-ttu-id="cc46b-243">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc46b-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1388

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
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="cc46b-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc46b-244">Response</span></span>
<span data-ttu-id="cc46b-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cc46b-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1560

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
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```




