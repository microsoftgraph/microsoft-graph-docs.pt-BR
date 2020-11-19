---
title: Atualizar officeSuiteApp
description: Atualiza as propriedades de um objeto officeSuiteApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8cf410011f65c0b625e23366f7e6bc5e7e3211fe
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49247794"
---
# <a name="update-officesuiteapp"></a><span data-ttu-id="42033-103">Atualizar officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="42033-103">Update officeSuiteApp</span></span>

<span data-ttu-id="42033-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42033-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42033-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="42033-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42033-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42033-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42033-107">Atualiza as propriedades de um objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="42033-107">Update the properties of a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42033-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="42033-108">Prerequisites</span></span>
<span data-ttu-id="42033-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42033-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42033-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42033-111">Permission type</span></span>|<span data-ttu-id="42033-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="42033-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42033-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42033-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42033-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42033-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="42033-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42033-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42033-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42033-116">Not supported.</span></span>|
|<span data-ttu-id="42033-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42033-117">Application</span></span>|<span data-ttu-id="42033-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42033-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42033-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42033-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="42033-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42033-120">Request headers</span></span>
|<span data-ttu-id="42033-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="42033-121">Header</span></span>|<span data-ttu-id="42033-122">Valor</span><span class="sxs-lookup"><span data-stu-id="42033-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42033-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="42033-123">Authorization</span></span>|<span data-ttu-id="42033-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42033-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42033-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="42033-125">Accept</span></span>|<span data-ttu-id="42033-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42033-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42033-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42033-127">Request body</span></span>
<span data-ttu-id="42033-128">No corpo da solicitação, forneça uma representação JSON do objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="42033-128">In the request body, supply a JSON representation for the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

<span data-ttu-id="42033-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="42033-129">The following table shows the properties that are required when you create the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span></span>

|<span data-ttu-id="42033-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42033-130">Property</span></span>|<span data-ttu-id="42033-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="42033-131">Type</span></span>|<span data-ttu-id="42033-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="42033-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42033-133">id</span><span class="sxs-lookup"><span data-stu-id="42033-133">id</span></span>|<span data-ttu-id="42033-134">String</span><span class="sxs-lookup"><span data-stu-id="42033-134">String</span></span>|<span data-ttu-id="42033-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="42033-135">Key of the entity.</span></span> <span data-ttu-id="42033-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42033-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42033-137">displayName</span><span class="sxs-lookup"><span data-stu-id="42033-137">displayName</span></span>|<span data-ttu-id="42033-138">String</span><span class="sxs-lookup"><span data-stu-id="42033-138">String</span></span>|<span data-ttu-id="42033-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="42033-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="42033-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42033-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42033-141">description</span><span class="sxs-lookup"><span data-stu-id="42033-141">description</span></span>|<span data-ttu-id="42033-142">String</span><span class="sxs-lookup"><span data-stu-id="42033-142">String</span></span>|<span data-ttu-id="42033-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="42033-143">The description of the app.</span></span> <span data-ttu-id="42033-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42033-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42033-145">publicador</span><span class="sxs-lookup"><span data-stu-id="42033-145">publisher</span></span>|<span data-ttu-id="42033-146">String</span><span class="sxs-lookup"><span data-stu-id="42033-146">String</span></span>|<span data-ttu-id="42033-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="42033-147">The publisher of the app.</span></span> <span data-ttu-id="42033-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42033-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42033-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="42033-149">largeIcon</span></span>|[<span data-ttu-id="42033-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="42033-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="42033-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="42033-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="42033-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42033-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42033-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42033-153">createdDateTime</span></span>|<span data-ttu-id="42033-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42033-154">DateTimeOffset</span></span>|<span data-ttu-id="42033-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="42033-155">The date and time the app was created.</span></span> <span data-ttu-id="42033-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42033-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42033-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="42033-157">lastModifiedDateTime</span></span>|<span data-ttu-id="42033-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42033-158">DateTimeOffset</span></span>|<span data-ttu-id="42033-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="42033-159">The date and time the app was last modified.</span></span> <span data-ttu-id="42033-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42033-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42033-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="42033-161">isFeatured</span></span>|<span data-ttu-id="42033-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="42033-162">Boolean</span></span>|<span data-ttu-id="42033-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42033-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42033-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="42033-164">privacyInformationUrl</span></span>|<span data-ttu-id="42033-165">String</span><span class="sxs-lookup"><span data-stu-id="42033-165">String</span></span>|<span data-ttu-id="42033-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="42033-166">The privacy statement Url.</span></span> <span data-ttu-id="42033-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42033-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42033-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="42033-168">informationUrl</span></span>|<span data-ttu-id="42033-169">String</span><span class="sxs-lookup"><span data-stu-id="42033-169">String</span></span>|<span data-ttu-id="42033-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="42033-170">The more information Url.</span></span> <span data-ttu-id="42033-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42033-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42033-172">owner</span><span class="sxs-lookup"><span data-stu-id="42033-172">owner</span></span>|<span data-ttu-id="42033-173">String</span><span class="sxs-lookup"><span data-stu-id="42033-173">String</span></span>|<span data-ttu-id="42033-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="42033-174">The owner of the app.</span></span> <span data-ttu-id="42033-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42033-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42033-176">developer</span><span class="sxs-lookup"><span data-stu-id="42033-176">developer</span></span>|<span data-ttu-id="42033-177">String</span><span class="sxs-lookup"><span data-stu-id="42033-177">String</span></span>|<span data-ttu-id="42033-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="42033-178">The developer of the app.</span></span> <span data-ttu-id="42033-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42033-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42033-180">notes</span><span class="sxs-lookup"><span data-stu-id="42033-180">notes</span></span>|<span data-ttu-id="42033-181">String</span><span class="sxs-lookup"><span data-stu-id="42033-181">String</span></span>|<span data-ttu-id="42033-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="42033-182">Notes for the app.</span></span> <span data-ttu-id="42033-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42033-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42033-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="42033-184">uploadState</span></span>|<span data-ttu-id="42033-185">Int32</span><span class="sxs-lookup"><span data-stu-id="42033-185">Int32</span></span>|<span data-ttu-id="42033-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="42033-186">The upload state.</span></span> <span data-ttu-id="42033-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="42033-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="42033-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42033-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42033-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="42033-189">publishingState</span></span>|[<span data-ttu-id="42033-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="42033-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="42033-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="42033-191">The publishing state for the app.</span></span> <span data-ttu-id="42033-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="42033-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="42033-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="42033-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="42033-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="42033-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="42033-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="42033-195">isAssigned</span></span>|<span data-ttu-id="42033-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="42033-196">Boolean</span></span>|<span data-ttu-id="42033-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="42033-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="42033-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42033-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42033-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="42033-199">roleScopeTagIds</span></span>|<span data-ttu-id="42033-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="42033-200">String collection</span></span>|<span data-ttu-id="42033-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="42033-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="42033-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42033-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42033-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="42033-203">dependentAppCount</span></span>|<span data-ttu-id="42033-204">Int32</span><span class="sxs-lookup"><span data-stu-id="42033-204">Int32</span></span>|<span data-ttu-id="42033-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="42033-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="42033-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42033-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42033-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="42033-207">supersedingAppCount</span></span>|<span data-ttu-id="42033-208">Int32</span><span class="sxs-lookup"><span data-stu-id="42033-208">Int32</span></span>|<span data-ttu-id="42033-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="42033-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="42033-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42033-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42033-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="42033-211">supersededAppCount</span></span>|<span data-ttu-id="42033-212">Int32</span><span class="sxs-lookup"><span data-stu-id="42033-212">Int32</span></span>|<span data-ttu-id="42033-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="42033-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="42033-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="42033-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="42033-215">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="42033-215">autoAcceptEula</span></span>|<span data-ttu-id="42033-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="42033-216">Boolean</span></span>|<span data-ttu-id="42033-217">O valor para aceitar o EULA automaticamente no dispositivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="42033-217">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="42033-218">productIds</span><span class="sxs-lookup"><span data-stu-id="42033-218">productIds</span></span>|<span data-ttu-id="42033-219">coleção [officeProductId](../resources/intune-apps-officeproductid.md)</span><span class="sxs-lookup"><span data-stu-id="42033-219">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="42033-220">As IDs de produto que representam a SKU do pacote do office365.</span><span class="sxs-lookup"><span data-stu-id="42033-220">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="42033-221">Os valores possíveis são: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span><span class="sxs-lookup"><span data-stu-id="42033-221">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="42033-222">excludedApps</span><span class="sxs-lookup"><span data-stu-id="42033-222">excludedApps</span></span>|[<span data-ttu-id="42033-223">excludedApps</span><span class="sxs-lookup"><span data-stu-id="42033-223">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="42033-224">A propriedade para representar os aplicativos que são excluídos da ID de produto do Office365 selecionado.</span><span class="sxs-lookup"><span data-stu-id="42033-224">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="42033-225">Propriedades usesharedcomputeractivation</span><span class="sxs-lookup"><span data-stu-id="42033-225">useSharedComputerActivation</span></span>|<span data-ttu-id="42033-226">Booliano</span><span class="sxs-lookup"><span data-stu-id="42033-226">Boolean</span></span>|<span data-ttu-id="42033-227">A propriedade que representa se a ativação de computador compartilhado é usada não para o pacote de aplicativos do office365.</span><span class="sxs-lookup"><span data-stu-id="42033-227">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="42033-228">updateChannel</span><span class="sxs-lookup"><span data-stu-id="42033-228">updateChannel</span></span>|[<span data-ttu-id="42033-229">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="42033-229">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="42033-230">A propriedade para representar o canal de atualização do office365.</span><span class="sxs-lookup"><span data-stu-id="42033-230">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="42033-231">Os possíveis valores são: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`, `monthlyEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="42033-231">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`, `monthlyEnterprise`.</span></span>|
|<span data-ttu-id="42033-232">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="42033-232">officePlatformArchitecture</span></span>|[<span data-ttu-id="42033-233">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="42033-233">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="42033-234">A propriedade para representar a versão do pacote de aplicativos do office365.</span><span class="sxs-lookup"><span data-stu-id="42033-234">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="42033-235">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="42033-235">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="42033-236">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="42033-236">localesToInstall</span></span>|<span data-ttu-id="42033-237">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="42033-237">String collection</span></span>|<span data-ttu-id="42033-238">A propriedade para representar os locais que são instalados quando os aplicativos do Office365 estão instalados.</span><span class="sxs-lookup"><span data-stu-id="42033-238">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="42033-239">Ele usa RFC 6033 padrão.</span><span class="sxs-lookup"><span data-stu-id="42033-239">It uses standard RFC 6033.</span></span> <span data-ttu-id="42033-240">Ref https://technet.microsoft.com/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="42033-240">Ref: https://technet.microsoft.com/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="42033-241">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="42033-241">installProgressDisplayLevel</span></span>|[<span data-ttu-id="42033-242">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="42033-242">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="42033-243">Para especificar o nível de exibição da interface do usuário da configuração de progresso da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="42033-243">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="42033-244">Os valores possíveis são: `none` e `full`.</span><span class="sxs-lookup"><span data-stu-id="42033-244">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="42033-245">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="42033-245">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="42033-246">Booliano</span><span class="sxs-lookup"><span data-stu-id="42033-246">Boolean</span></span>|<span data-ttu-id="42033-247">A propriedade para determinar se deve desinstalar o Office MSI existente se um pacote de aplicativos do Office365 for implantado no dispositivo ou não.</span><span class="sxs-lookup"><span data-stu-id="42033-247">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="42033-248">targetVersion</span><span class="sxs-lookup"><span data-stu-id="42033-248">targetVersion</span></span>|<span data-ttu-id="42033-249">String</span><span class="sxs-lookup"><span data-stu-id="42033-249">String</span></span>|<span data-ttu-id="42033-250">A propriedade para representar a versão de destino específica para o pacote de aplicativos do Office365 que deve permanecer implantado nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="42033-250">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="42033-251">updateVersion</span><span class="sxs-lookup"><span data-stu-id="42033-251">updateVersion</span></span>|<span data-ttu-id="42033-252">String</span><span class="sxs-lookup"><span data-stu-id="42033-252">String</span></span>|<span data-ttu-id="42033-253">A propriedade para representar a versão de atualização na qual a versão de destino específica está disponível para o pacote de aplicativos do office365.</span><span class="sxs-lookup"><span data-stu-id="42033-253">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="42033-254">officeConfigurationXml</span><span class="sxs-lookup"><span data-stu-id="42033-254">officeConfigurationXml</span></span>|<span data-ttu-id="42033-255">Binária</span><span class="sxs-lookup"><span data-stu-id="42033-255">Binary</span></span>|<span data-ttu-id="42033-256">A propriedade para representar o arquivo de configuração XML que pode ser especificado para aplicativos do Office ProPlus.</span><span class="sxs-lookup"><span data-stu-id="42033-256">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="42033-257">Tem precedência sobre todas as outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="42033-257">Takes precedence over all other properties.</span></span> <span data-ttu-id="42033-258">Quando presente, o arquivo de configuração XML será usado para criar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="42033-258">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="42033-259">Resposta</span><span class="sxs-lookup"><span data-stu-id="42033-259">Response</span></span>
<span data-ttu-id="42033-260">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42033-260">If successful, this method returns a `200 OK` response code and an updated [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42033-261">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42033-261">Example</span></span>

### <a name="request"></a><span data-ttu-id="42033-262">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42033-262">Request</span></span>
<span data-ttu-id="42033-263">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42033-263">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1675

{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "bing": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "teams": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value",
  "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="42033-264">Resposta</span><span class="sxs-lookup"><span data-stu-id="42033-264">Response</span></span>
<span data-ttu-id="42033-p127">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42033-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1847

{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
  "id": "9b263b46-3b46-9b26-463b-269b463b269b",
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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "bing": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "teams": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value",
  "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
}
```




