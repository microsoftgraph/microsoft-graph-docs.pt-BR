---
title: Atualizar windowsUniversalAppX
description: Atualiza as propriedades de um objeto windowsUniversalAppX.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1b9f1acc65a0c6f29a9f0f383af60b61524a9a0b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163284"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="db947-103">Atualizar windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="db947-103">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="db947-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="db947-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db947-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="db947-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db947-106">Atualiza as propriedades de um objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="db947-106">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db947-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="db947-107">Prerequisites</span></span>
<span data-ttu-id="db947-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="db947-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="db947-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db947-110">Permission type</span></span>|<span data-ttu-id="db947-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="db947-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db947-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db947-112">Delegated (work or school account)</span></span>|<span data-ttu-id="db947-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db947-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="db947-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db947-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db947-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db947-115">Not supported.</span></span>|
|<span data-ttu-id="db947-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db947-116">Application</span></span>|<span data-ttu-id="db947-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db947-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db947-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db947-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="db947-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db947-119">Request headers</span></span>
|<span data-ttu-id="db947-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="db947-120">Header</span></span>|<span data-ttu-id="db947-121">Valor</span><span class="sxs-lookup"><span data-stu-id="db947-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db947-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="db947-122">Authorization</span></span>|<span data-ttu-id="db947-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db947-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db947-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="db947-124">Accept</span></span>|<span data-ttu-id="db947-125">application/json</span><span class="sxs-lookup"><span data-stu-id="db947-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db947-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db947-126">Request body</span></span>
<span data-ttu-id="db947-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="db947-127">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="db947-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="db947-128">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="db947-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db947-129">Property</span></span>|<span data-ttu-id="db947-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="db947-130">Type</span></span>|<span data-ttu-id="db947-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="db947-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db947-132">id</span><span class="sxs-lookup"><span data-stu-id="db947-132">id</span></span>|<span data-ttu-id="db947-133">String</span><span class="sxs-lookup"><span data-stu-id="db947-133">String</span></span>|<span data-ttu-id="db947-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="db947-134">Key of the entity.</span></span> <span data-ttu-id="db947-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db947-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db947-136">displayName</span><span class="sxs-lookup"><span data-stu-id="db947-136">displayName</span></span>|<span data-ttu-id="db947-137">String</span><span class="sxs-lookup"><span data-stu-id="db947-137">String</span></span>|<span data-ttu-id="db947-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="db947-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="db947-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db947-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db947-140">description</span><span class="sxs-lookup"><span data-stu-id="db947-140">description</span></span>|<span data-ttu-id="db947-141">String</span><span class="sxs-lookup"><span data-stu-id="db947-141">String</span></span>|<span data-ttu-id="db947-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="db947-142">The description of the app.</span></span> <span data-ttu-id="db947-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db947-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db947-144">publisher</span><span class="sxs-lookup"><span data-stu-id="db947-144">publisher</span></span>|<span data-ttu-id="db947-145">String</span><span class="sxs-lookup"><span data-stu-id="db947-145">String</span></span>|<span data-ttu-id="db947-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="db947-146">The publisher of the app.</span></span> <span data-ttu-id="db947-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db947-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db947-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="db947-148">largeIcon</span></span>|[<span data-ttu-id="db947-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="db947-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="db947-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="db947-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="db947-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db947-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db947-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="db947-152">createdDateTime</span></span>|<span data-ttu-id="db947-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db947-153">DateTimeOffset</span></span>|<span data-ttu-id="db947-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="db947-154">The date and time the app was created.</span></span> <span data-ttu-id="db947-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db947-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db947-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db947-156">lastModifiedDateTime</span></span>|<span data-ttu-id="db947-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db947-157">DateTimeOffset</span></span>|<span data-ttu-id="db947-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="db947-158">The date and time the app was last modified.</span></span> <span data-ttu-id="db947-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db947-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db947-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="db947-160">isFeatured</span></span>|<span data-ttu-id="db947-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="db947-161">Boolean</span></span>|<span data-ttu-id="db947-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db947-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db947-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="db947-163">privacyInformationUrl</span></span>|<span data-ttu-id="db947-164">String</span><span class="sxs-lookup"><span data-stu-id="db947-164">String</span></span>|<span data-ttu-id="db947-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="db947-165">The privacy statement Url.</span></span> <span data-ttu-id="db947-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db947-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db947-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="db947-167">informationUrl</span></span>|<span data-ttu-id="db947-168">String</span><span class="sxs-lookup"><span data-stu-id="db947-168">String</span></span>|<span data-ttu-id="db947-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="db947-169">The more information Url.</span></span> <span data-ttu-id="db947-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db947-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db947-171">owner</span><span class="sxs-lookup"><span data-stu-id="db947-171">owner</span></span>|<span data-ttu-id="db947-172">String</span><span class="sxs-lookup"><span data-stu-id="db947-172">String</span></span>|<span data-ttu-id="db947-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="db947-173">The owner of the app.</span></span> <span data-ttu-id="db947-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db947-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db947-175">developer</span><span class="sxs-lookup"><span data-stu-id="db947-175">developer</span></span>|<span data-ttu-id="db947-176">String</span><span class="sxs-lookup"><span data-stu-id="db947-176">String</span></span>|<span data-ttu-id="db947-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="db947-177">The developer of the app.</span></span> <span data-ttu-id="db947-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db947-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db947-179">Observações</span><span class="sxs-lookup"><span data-stu-id="db947-179">notes</span></span>|<span data-ttu-id="db947-180">String</span><span class="sxs-lookup"><span data-stu-id="db947-180">String</span></span>|<span data-ttu-id="db947-181">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="db947-181">Notes for the app.</span></span> <span data-ttu-id="db947-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db947-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db947-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="db947-183">uploadState</span></span>|<span data-ttu-id="db947-184">Int32</span><span class="sxs-lookup"><span data-stu-id="db947-184">Int32</span></span>|<span data-ttu-id="db947-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="db947-185">The upload state.</span></span> <span data-ttu-id="db947-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db947-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db947-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="db947-187">publishingState</span></span>|[<span data-ttu-id="db947-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="db947-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="db947-189">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="db947-189">The publishing state for the app.</span></span> <span data-ttu-id="db947-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="db947-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="db947-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="db947-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="db947-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="db947-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="db947-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="db947-193">isAssigned</span></span>|<span data-ttu-id="db947-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="db947-194">Boolean</span></span>|<span data-ttu-id="db947-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="db947-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="db947-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db947-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db947-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="db947-197">roleScopeTagIds</span></span>|<span data-ttu-id="db947-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="db947-198">String collection</span></span>|<span data-ttu-id="db947-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="db947-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="db947-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db947-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db947-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="db947-201">committedContentVersion</span></span>|<span data-ttu-id="db947-202">String</span><span class="sxs-lookup"><span data-stu-id="db947-202">String</span></span>|<span data-ttu-id="db947-203">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="db947-203">The internal committed content version.</span></span> <span data-ttu-id="db947-204">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="db947-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="db947-205">fileName</span><span class="sxs-lookup"><span data-stu-id="db947-205">fileName</span></span>|<span data-ttu-id="db947-206">String</span><span class="sxs-lookup"><span data-stu-id="db947-206">String</span></span>|<span data-ttu-id="db947-207">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="db947-207">The name of the main Lob application file.</span></span> <span data-ttu-id="db947-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="db947-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="db947-209">size</span><span class="sxs-lookup"><span data-stu-id="db947-209">size</span></span>|<span data-ttu-id="db947-210">Int64</span><span class="sxs-lookup"><span data-stu-id="db947-210">Int64</span></span>|<span data-ttu-id="db947-211">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="db947-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="db947-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="db947-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="db947-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="db947-213">applicableArchitectures</span></span>|[<span data-ttu-id="db947-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="db947-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="db947-215">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="db947-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="db947-216">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="db947-216">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="db947-217">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="db947-217">applicableDeviceTypes</span></span>|[<span data-ttu-id="db947-218">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="db947-218">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="db947-219">Os tipos de dispositivos Windows nos quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="db947-219">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="db947-220">Os valores possíveis são: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="db947-220">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="db947-221">identityName</span><span class="sxs-lookup"><span data-stu-id="db947-221">identityName</span></span>|<span data-ttu-id="db947-222">String</span><span class="sxs-lookup"><span data-stu-id="db947-222">String</span></span>|<span data-ttu-id="db947-223">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="db947-223">The Identity Name.</span></span>|
|<span data-ttu-id="db947-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="db947-224">identityPublisherHash</span></span>|<span data-ttu-id="db947-225">String</span><span class="sxs-lookup"><span data-stu-id="db947-225">String</span></span>|<span data-ttu-id="db947-226">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="db947-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="db947-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="db947-227">identityResourceIdentifier</span></span>|<span data-ttu-id="db947-228">String</span><span class="sxs-lookup"><span data-stu-id="db947-228">String</span></span>|<span data-ttu-id="db947-229">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="db947-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="db947-230">isBundle</span><span class="sxs-lookup"><span data-stu-id="db947-230">isBundle</span></span>|<span data-ttu-id="db947-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="db947-231">Boolean</span></span>|<span data-ttu-id="db947-232">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="db947-232">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="db947-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="db947-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="db947-234">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="db947-234">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="db947-235">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="db947-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="db947-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="db947-236">identityVersion</span></span>|<span data-ttu-id="db947-237">String</span><span class="sxs-lookup"><span data-stu-id="db947-237">String</span></span>|<span data-ttu-id="db947-238">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="db947-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="db947-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="db947-239">Response</span></span>
<span data-ttu-id="db947-240">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db947-240">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db947-241">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db947-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="db947-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db947-242">Request</span></span>
<span data-ttu-id="db947-243">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db947-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="db947-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="db947-244">Response</span></span>
<span data-ttu-id="db947-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db947-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




