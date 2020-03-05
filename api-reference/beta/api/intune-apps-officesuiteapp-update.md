---
title: Atualizar officeSuiteApp
description: Atualiza as propriedades de um objeto officeSuiteApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8badffb9a84411a00eaa9a52d194c3b431ef7812
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450633"
---
# <a name="update-officesuiteapp"></a><span data-ttu-id="53feb-103">Atualizar officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="53feb-103">Update officeSuiteApp</span></span>

<span data-ttu-id="53feb-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="53feb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53feb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="53feb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53feb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="53feb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53feb-107">Atualiza as propriedades de um objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="53feb-107">Update the properties of a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53feb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="53feb-108">Prerequisites</span></span>
<span data-ttu-id="53feb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53feb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53feb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53feb-111">Permission type</span></span>|<span data-ttu-id="53feb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="53feb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53feb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53feb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53feb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53feb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="53feb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53feb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53feb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53feb-116">Not supported.</span></span>|
|<span data-ttu-id="53feb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53feb-117">Application</span></span>|<span data-ttu-id="53feb-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53feb-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53feb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53feb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="53feb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53feb-120">Request headers</span></span>
|<span data-ttu-id="53feb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="53feb-121">Header</span></span>|<span data-ttu-id="53feb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="53feb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53feb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="53feb-123">Authorization</span></span>|<span data-ttu-id="53feb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53feb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53feb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="53feb-125">Accept</span></span>|<span data-ttu-id="53feb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53feb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53feb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53feb-127">Request body</span></span>
<span data-ttu-id="53feb-128">No corpo da solicitação, forneça uma representação JSON do objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="53feb-128">In the request body, supply a JSON representation for the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

<span data-ttu-id="53feb-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="53feb-129">The following table shows the properties that are required when you create the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span></span>

|<span data-ttu-id="53feb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53feb-130">Property</span></span>|<span data-ttu-id="53feb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="53feb-131">Type</span></span>|<span data-ttu-id="53feb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="53feb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53feb-133">id</span><span class="sxs-lookup"><span data-stu-id="53feb-133">id</span></span>|<span data-ttu-id="53feb-134">String</span><span class="sxs-lookup"><span data-stu-id="53feb-134">String</span></span>|<span data-ttu-id="53feb-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="53feb-135">Key of the entity.</span></span> <span data-ttu-id="53feb-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53feb-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53feb-137">displayName</span><span class="sxs-lookup"><span data-stu-id="53feb-137">displayName</span></span>|<span data-ttu-id="53feb-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53feb-138">String</span></span>|<span data-ttu-id="53feb-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="53feb-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="53feb-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53feb-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53feb-141">description</span><span class="sxs-lookup"><span data-stu-id="53feb-141">description</span></span>|<span data-ttu-id="53feb-142">String</span><span class="sxs-lookup"><span data-stu-id="53feb-142">String</span></span>|<span data-ttu-id="53feb-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53feb-143">The description of the app.</span></span> <span data-ttu-id="53feb-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53feb-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53feb-145">publicador</span><span class="sxs-lookup"><span data-stu-id="53feb-145">publisher</span></span>|<span data-ttu-id="53feb-146">String</span><span class="sxs-lookup"><span data-stu-id="53feb-146">String</span></span>|<span data-ttu-id="53feb-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53feb-147">The publisher of the app.</span></span> <span data-ttu-id="53feb-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53feb-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53feb-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="53feb-149">largeIcon</span></span>|[<span data-ttu-id="53feb-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="53feb-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="53feb-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="53feb-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="53feb-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53feb-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53feb-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="53feb-153">createdDateTime</span></span>|<span data-ttu-id="53feb-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53feb-154">DateTimeOffset</span></span>|<span data-ttu-id="53feb-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53feb-155">The date and time the app was created.</span></span> <span data-ttu-id="53feb-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53feb-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53feb-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53feb-157">lastModifiedDateTime</span></span>|<span data-ttu-id="53feb-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53feb-158">DateTimeOffset</span></span>|<span data-ttu-id="53feb-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="53feb-159">The date and time the app was last modified.</span></span> <span data-ttu-id="53feb-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53feb-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53feb-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="53feb-161">isFeatured</span></span>|<span data-ttu-id="53feb-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="53feb-162">Boolean</span></span>|<span data-ttu-id="53feb-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53feb-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53feb-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="53feb-164">privacyInformationUrl</span></span>|<span data-ttu-id="53feb-165">String</span><span class="sxs-lookup"><span data-stu-id="53feb-165">String</span></span>|<span data-ttu-id="53feb-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="53feb-166">The privacy statement Url.</span></span> <span data-ttu-id="53feb-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53feb-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53feb-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="53feb-168">informationUrl</span></span>|<span data-ttu-id="53feb-169">String</span><span class="sxs-lookup"><span data-stu-id="53feb-169">String</span></span>|<span data-ttu-id="53feb-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="53feb-170">The more information Url.</span></span> <span data-ttu-id="53feb-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53feb-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53feb-172">owner</span><span class="sxs-lookup"><span data-stu-id="53feb-172">owner</span></span>|<span data-ttu-id="53feb-173">String</span><span class="sxs-lookup"><span data-stu-id="53feb-173">String</span></span>|<span data-ttu-id="53feb-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="53feb-174">The owner of the app.</span></span> <span data-ttu-id="53feb-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53feb-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53feb-176">developer</span><span class="sxs-lookup"><span data-stu-id="53feb-176">developer</span></span>|<span data-ttu-id="53feb-177">String</span><span class="sxs-lookup"><span data-stu-id="53feb-177">String</span></span>|<span data-ttu-id="53feb-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53feb-178">The developer of the app.</span></span> <span data-ttu-id="53feb-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53feb-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53feb-180">notes</span><span class="sxs-lookup"><span data-stu-id="53feb-180">notes</span></span>|<span data-ttu-id="53feb-181">String</span><span class="sxs-lookup"><span data-stu-id="53feb-181">String</span></span>|<span data-ttu-id="53feb-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53feb-182">Notes for the app.</span></span> <span data-ttu-id="53feb-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53feb-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53feb-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="53feb-184">uploadState</span></span>|<span data-ttu-id="53feb-185">Int32</span><span class="sxs-lookup"><span data-stu-id="53feb-185">Int32</span></span>|<span data-ttu-id="53feb-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="53feb-186">The upload state.</span></span> <span data-ttu-id="53feb-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53feb-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53feb-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="53feb-188">publishingState</span></span>|[<span data-ttu-id="53feb-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="53feb-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="53feb-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53feb-190">The publishing state for the app.</span></span> <span data-ttu-id="53feb-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="53feb-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="53feb-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53feb-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="53feb-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="53feb-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="53feb-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="53feb-194">isAssigned</span></span>|<span data-ttu-id="53feb-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="53feb-195">Boolean</span></span>|<span data-ttu-id="53feb-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="53feb-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="53feb-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53feb-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53feb-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="53feb-198">roleScopeTagIds</span></span>|<span data-ttu-id="53feb-199">String collection</span><span class="sxs-lookup"><span data-stu-id="53feb-199">String collection</span></span>|<span data-ttu-id="53feb-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="53feb-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="53feb-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53feb-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53feb-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="53feb-202">dependentAppCount</span></span>|<span data-ttu-id="53feb-203">Int32</span><span class="sxs-lookup"><span data-stu-id="53feb-203">Int32</span></span>|<span data-ttu-id="53feb-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="53feb-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="53feb-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53feb-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53feb-206">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="53feb-206">autoAcceptEula</span></span>|<span data-ttu-id="53feb-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="53feb-207">Boolean</span></span>|<span data-ttu-id="53feb-208">O valor para aceitar o EULA automaticamente no dispositivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="53feb-208">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="53feb-209">productIds</span><span class="sxs-lookup"><span data-stu-id="53feb-209">productIds</span></span>|<span data-ttu-id="53feb-210">coleção [officeProductId](../resources/intune-apps-officeproductid.md)</span><span class="sxs-lookup"><span data-stu-id="53feb-210">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="53feb-211">As IDs de produto que representam a SKU do pacote do office365.</span><span class="sxs-lookup"><span data-stu-id="53feb-211">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="53feb-212">Os valores possíveis são: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span><span class="sxs-lookup"><span data-stu-id="53feb-212">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="53feb-213">excludedApps</span><span class="sxs-lookup"><span data-stu-id="53feb-213">excludedApps</span></span>|[<span data-ttu-id="53feb-214">excludedApps</span><span class="sxs-lookup"><span data-stu-id="53feb-214">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="53feb-215">A propriedade para representar os aplicativos que são excluídos da ID de produto do Office365 selecionado.</span><span class="sxs-lookup"><span data-stu-id="53feb-215">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="53feb-216">Propriedades usesharedcomputeractivation</span><span class="sxs-lookup"><span data-stu-id="53feb-216">useSharedComputerActivation</span></span>|<span data-ttu-id="53feb-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="53feb-217">Boolean</span></span>|<span data-ttu-id="53feb-218">A propriedade que representa se a ativação de computador compartilhado é usada não para o pacote de aplicativos do office365.</span><span class="sxs-lookup"><span data-stu-id="53feb-218">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="53feb-219">updateChannel</span><span class="sxs-lookup"><span data-stu-id="53feb-219">updateChannel</span></span>|[<span data-ttu-id="53feb-220">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="53feb-220">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="53feb-221">A propriedade para representar o canal de atualização do office365.</span><span class="sxs-lookup"><span data-stu-id="53feb-221">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="53feb-222">Os valores possíveis são: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span><span class="sxs-lookup"><span data-stu-id="53feb-222">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="53feb-223">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="53feb-223">officePlatformArchitecture</span></span>|[<span data-ttu-id="53feb-224">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="53feb-224">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="53feb-225">A propriedade para representar a versão do pacote de aplicativos do office365.</span><span class="sxs-lookup"><span data-stu-id="53feb-225">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="53feb-226">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="53feb-226">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="53feb-227">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="53feb-227">localesToInstall</span></span>|<span data-ttu-id="53feb-228">String collection</span><span class="sxs-lookup"><span data-stu-id="53feb-228">String collection</span></span>|<span data-ttu-id="53feb-229">A propriedade para representar os locais que são instalados quando os aplicativos do Office365 estão instalados.</span><span class="sxs-lookup"><span data-stu-id="53feb-229">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="53feb-230">Ele usa RFC 6033 padrão.</span><span class="sxs-lookup"><span data-stu-id="53feb-230">It uses standard RFC 6033.</span></span> <span data-ttu-id="53feb-231">Refhttps://technet.microsoft.com/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="53feb-231">Ref: https://technet.microsoft.com/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="53feb-232">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="53feb-232">installProgressDisplayLevel</span></span>|[<span data-ttu-id="53feb-233">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="53feb-233">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="53feb-234">Para especificar o nível de exibição da interface do usuário da configuração de progresso da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="53feb-234">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="53feb-235">Os valores possíveis são: `none` e `full`.</span><span class="sxs-lookup"><span data-stu-id="53feb-235">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="53feb-236">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="53feb-236">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="53feb-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="53feb-237">Boolean</span></span>|<span data-ttu-id="53feb-238">A propriedade para determinar se deve desinstalar o Office MSI existente se um pacote de aplicativos do Office365 for implantado no dispositivo ou não.</span><span class="sxs-lookup"><span data-stu-id="53feb-238">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="53feb-239">targetVersion</span><span class="sxs-lookup"><span data-stu-id="53feb-239">targetVersion</span></span>|<span data-ttu-id="53feb-240">String</span><span class="sxs-lookup"><span data-stu-id="53feb-240">String</span></span>|<span data-ttu-id="53feb-241">A propriedade para representar a versão de destino específica para o pacote de aplicativos do Office365 que deve permanecer implantado nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="53feb-241">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="53feb-242">updateVersion</span><span class="sxs-lookup"><span data-stu-id="53feb-242">updateVersion</span></span>|<span data-ttu-id="53feb-243">String</span><span class="sxs-lookup"><span data-stu-id="53feb-243">String</span></span>|<span data-ttu-id="53feb-244">A propriedade para representar a versão de atualização na qual a versão de destino específica está disponível para o pacote de aplicativos do office365.</span><span class="sxs-lookup"><span data-stu-id="53feb-244">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="53feb-245">officeConfigurationXml</span><span class="sxs-lookup"><span data-stu-id="53feb-245">officeConfigurationXml</span></span>|<span data-ttu-id="53feb-246">Binária</span><span class="sxs-lookup"><span data-stu-id="53feb-246">Binary</span></span>|<span data-ttu-id="53feb-247">A propriedade para representar o arquivo de configuração XML que pode ser especificado para aplicativos do Office ProPlus.</span><span class="sxs-lookup"><span data-stu-id="53feb-247">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="53feb-248">Tem precedência sobre todas as outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="53feb-248">Takes precedence over all other properties.</span></span> <span data-ttu-id="53feb-249">Quando presente, o arquivo de configuração XML será usado para criar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53feb-249">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="53feb-250">Resposta</span><span class="sxs-lookup"><span data-stu-id="53feb-250">Response</span></span>
<span data-ttu-id="53feb-251">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53feb-251">If successful, this method returns a `200 OK` response code and an updated [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53feb-252">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53feb-252">Example</span></span>

### <a name="request"></a><span data-ttu-id="53feb-253">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53feb-253">Request</span></span>
<span data-ttu-id="53feb-254">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53feb-254">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1599

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
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
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

### <a name="response"></a><span data-ttu-id="53feb-255">Resposta</span><span class="sxs-lookup"><span data-stu-id="53feb-255">Response</span></span>
<span data-ttu-id="53feb-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53feb-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1771

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
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
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





