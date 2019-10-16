---
title: Atualizar macOsVppApp
description: Atualiza as propriedades de um objeto macOsVppApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2048f8e6c30d64dfd74b8a8f922138e63efb798e
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535286"
---
# <a name="update-macosvppapp"></a><span data-ttu-id="f2153-103">Atualizar macOsVppApp</span><span class="sxs-lookup"><span data-stu-id="f2153-103">Update macOsVppApp</span></span>

> <span data-ttu-id="f2153-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f2153-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2153-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2153-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2153-106">Atualiza as propriedades de um objeto [macOsVppApp](../resources/intune-apps-macosvppapp.md) .</span><span class="sxs-lookup"><span data-stu-id="f2153-106">Update the properties of a [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2153-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2153-107">Prerequisites</span></span>
<span data-ttu-id="f2153-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2153-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2153-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2153-110">Permission type</span></span>|<span data-ttu-id="f2153-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2153-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2153-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2153-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f2153-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2153-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f2153-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2153-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2153-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2153-115">Not supported.</span></span>|
|<span data-ttu-id="f2153-116">Application</span><span class="sxs-lookup"><span data-stu-id="f2153-116">Application</span></span>|<span data-ttu-id="f2153-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2153-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2153-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2153-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f2153-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2153-119">Request headers</span></span>
|<span data-ttu-id="f2153-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2153-120">Header</span></span>|<span data-ttu-id="f2153-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f2153-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2153-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2153-122">Authorization</span></span>|<span data-ttu-id="f2153-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2153-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2153-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2153-124">Accept</span></span>|<span data-ttu-id="f2153-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f2153-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2153-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2153-126">Request body</span></span>
<span data-ttu-id="f2153-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOsVppApp](../resources/intune-apps-macosvppapp.md) .</span><span class="sxs-lookup"><span data-stu-id="f2153-127">In the request body, supply a JSON representation for the [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

<span data-ttu-id="f2153-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOsVppApp](../resources/intune-apps-macosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2153-128">The following table shows the properties that are required when you create the [macOsVppApp](../resources/intune-apps-macosvppapp.md).</span></span>

|<span data-ttu-id="f2153-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2153-129">Property</span></span>|<span data-ttu-id="f2153-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2153-130">Type</span></span>|<span data-ttu-id="f2153-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2153-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2153-132">id</span><span class="sxs-lookup"><span data-stu-id="f2153-132">id</span></span>|<span data-ttu-id="f2153-133">String</span><span class="sxs-lookup"><span data-stu-id="f2153-133">String</span></span>|<span data-ttu-id="f2153-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f2153-134">Key of the entity.</span></span> <span data-ttu-id="f2153-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2153-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2153-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f2153-136">displayName</span></span>|<span data-ttu-id="f2153-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2153-137">String</span></span>|<span data-ttu-id="f2153-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f2153-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f2153-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2153-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2153-140">description</span><span class="sxs-lookup"><span data-stu-id="f2153-140">description</span></span>|<span data-ttu-id="f2153-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2153-141">String</span></span>|<span data-ttu-id="f2153-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2153-142">The description of the app.</span></span> <span data-ttu-id="f2153-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2153-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2153-144">publicador</span><span class="sxs-lookup"><span data-stu-id="f2153-144">publisher</span></span>|<span data-ttu-id="f2153-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2153-145">String</span></span>|<span data-ttu-id="f2153-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2153-146">The publisher of the app.</span></span> <span data-ttu-id="f2153-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2153-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2153-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f2153-148">largeIcon</span></span>|[<span data-ttu-id="f2153-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f2153-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f2153-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="f2153-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f2153-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2153-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2153-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2153-152">createdDateTime</span></span>|<span data-ttu-id="f2153-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2153-153">DateTimeOffset</span></span>|<span data-ttu-id="f2153-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2153-154">The date and time the app was created.</span></span> <span data-ttu-id="f2153-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2153-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2153-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2153-156">lastModifiedDateTime</span></span>|<span data-ttu-id="f2153-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2153-157">DateTimeOffset</span></span>|<span data-ttu-id="f2153-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f2153-158">The date and time the app was last modified.</span></span> <span data-ttu-id="f2153-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2153-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2153-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f2153-160">isFeatured</span></span>|<span data-ttu-id="f2153-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2153-161">Boolean</span></span>|<span data-ttu-id="f2153-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2153-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2153-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f2153-163">privacyInformationUrl</span></span>|<span data-ttu-id="f2153-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2153-164">String</span></span>|<span data-ttu-id="f2153-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="f2153-165">The privacy statement Url.</span></span> <span data-ttu-id="f2153-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2153-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2153-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f2153-167">informationUrl</span></span>|<span data-ttu-id="f2153-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2153-168">String</span></span>|<span data-ttu-id="f2153-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="f2153-169">The more information Url.</span></span> <span data-ttu-id="f2153-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2153-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2153-171">owner</span><span class="sxs-lookup"><span data-stu-id="f2153-171">owner</span></span>|<span data-ttu-id="f2153-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2153-172">String</span></span>|<span data-ttu-id="f2153-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f2153-173">The owner of the app.</span></span> <span data-ttu-id="f2153-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2153-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2153-175">developer</span><span class="sxs-lookup"><span data-stu-id="f2153-175">developer</span></span>|<span data-ttu-id="f2153-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2153-176">String</span></span>|<span data-ttu-id="f2153-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2153-177">The developer of the app.</span></span> <span data-ttu-id="f2153-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2153-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2153-179">notes</span><span class="sxs-lookup"><span data-stu-id="f2153-179">notes</span></span>|<span data-ttu-id="f2153-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2153-180">String</span></span>|<span data-ttu-id="f2153-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2153-181">Notes for the app.</span></span> <span data-ttu-id="f2153-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2153-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2153-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="f2153-183">uploadState</span></span>|<span data-ttu-id="f2153-184">Int32</span><span class="sxs-lookup"><span data-stu-id="f2153-184">Int32</span></span>|<span data-ttu-id="f2153-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="f2153-185">The upload state.</span></span> <span data-ttu-id="f2153-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2153-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2153-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="f2153-187">publishingState</span></span>|[<span data-ttu-id="f2153-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f2153-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f2153-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2153-189">The publishing state for the app.</span></span> <span data-ttu-id="f2153-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="f2153-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f2153-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2153-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="f2153-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f2153-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f2153-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f2153-193">isAssigned</span></span>|<span data-ttu-id="f2153-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2153-194">Boolean</span></span>|<span data-ttu-id="f2153-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="f2153-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f2153-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2153-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2153-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f2153-197">roleScopeTagIds</span></span>|<span data-ttu-id="f2153-198">String collection</span><span class="sxs-lookup"><span data-stu-id="f2153-198">String collection</span></span>|<span data-ttu-id="f2153-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="f2153-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f2153-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2153-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2153-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="f2153-201">dependentAppCount</span></span>|<span data-ttu-id="f2153-202">Int32</span><span class="sxs-lookup"><span data-stu-id="f2153-202">Int32</span></span>|<span data-ttu-id="f2153-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="f2153-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="f2153-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2153-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2153-205">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f2153-205">usedLicenseCount</span></span>|<span data-ttu-id="f2153-206">Int32</span><span class="sxs-lookup"><span data-stu-id="f2153-206">Int32</span></span>|<span data-ttu-id="f2153-207">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="f2153-207">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="f2153-208">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f2153-208">totalLicenseCount</span></span>|<span data-ttu-id="f2153-209">Int32</span><span class="sxs-lookup"><span data-stu-id="f2153-209">Int32</span></span>|<span data-ttu-id="f2153-210">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="f2153-210">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="f2153-211">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="f2153-211">releaseDateTime</span></span>|<span data-ttu-id="f2153-212">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2153-212">DateTimeOffset</span></span>|<span data-ttu-id="f2153-213">A data e a hora de lançamento do aplicativo VPP.</span><span class="sxs-lookup"><span data-stu-id="f2153-213">The VPP application release date and time.</span></span>|
|<span data-ttu-id="f2153-214">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f2153-214">appStoreUrl</span></span>|<span data-ttu-id="f2153-215">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2153-215">String</span></span>|<span data-ttu-id="f2153-216">A URL da loja.</span><span class="sxs-lookup"><span data-stu-id="f2153-216">The store URL.</span></span>|
|<span data-ttu-id="f2153-217">licensingType</span><span class="sxs-lookup"><span data-stu-id="f2153-217">licensingType</span></span>|[<span data-ttu-id="f2153-218">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="f2153-218">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="f2153-219">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="f2153-219">The supported License Type.</span></span>|
|<span data-ttu-id="f2153-220">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="f2153-220">vppTokenOrganizationName</span></span>|<span data-ttu-id="f2153-221">String</span><span class="sxs-lookup"><span data-stu-id="f2153-221">String</span></span>|<span data-ttu-id="f2153-222">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="f2153-222">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="f2153-223">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="f2153-223">vppTokenAccountType</span></span>|[<span data-ttu-id="f2153-224">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="f2153-224">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="f2153-225">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="f2153-225">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="f2153-226">Os valores possíveis são: `business` e `education`.</span><span class="sxs-lookup"><span data-stu-id="f2153-226">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="f2153-227">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="f2153-227">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="f2153-228">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="f2153-228">vppTokenAppleId</span></span>|<span data-ttu-id="f2153-229">String</span><span class="sxs-lookup"><span data-stu-id="f2153-229">String</span></span>|<span data-ttu-id="f2153-230">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="f2153-230">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="f2153-231">bundleId</span><span class="sxs-lookup"><span data-stu-id="f2153-231">bundleId</span></span>|<span data-ttu-id="f2153-232">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2153-232">String</span></span>|<span data-ttu-id="f2153-233">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="f2153-233">The Identity Name.</span></span>|
|<span data-ttu-id="f2153-234">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="f2153-234">vppTokenId</span></span>|<span data-ttu-id="f2153-235">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2153-235">String</span></span>|<span data-ttu-id="f2153-236">Identificador do token VPP associado a este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2153-236">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="f2153-237">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="f2153-237">revokeLicenseActionResults</span></span>|<span data-ttu-id="f2153-238">coleção [macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f2153-238">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="f2153-239">Resultados da revogação de ações de licença neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2153-239">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="f2153-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2153-240">Response</span></span>
<span data-ttu-id="f2153-241">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [macOsVppApp](../resources/intune-apps-macosvppapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2153-241">If successful, this method returns a `200 OK` response code and an updated [macOsVppApp](../resources/intune-apps-macosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2153-242">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2153-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2153-243">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2153-243">Request</span></span>
<span data-ttu-id="f2153-244">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2153-244">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1869

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="f2153-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2153-245">Response</span></span>
<span data-ttu-id="f2153-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2153-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2041

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
  "id": "10b95265-5265-10b9-6552-b9106552b910",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```






