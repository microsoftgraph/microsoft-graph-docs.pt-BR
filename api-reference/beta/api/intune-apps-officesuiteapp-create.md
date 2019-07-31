---
title: Criar officeSuiteApp
description: Criar um novo objeto officeSuiteApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 664fc19eb20079c10352571e9d9d1cdb754bb7d8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960507"
---
# <a name="create-officesuiteapp"></a><span data-ttu-id="0019f-103">Criar officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="0019f-103">Create officeSuiteApp</span></span>

> <span data-ttu-id="0019f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0019f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0019f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0019f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0019f-106">Criar um novo objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="0019f-106">Create a new [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0019f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0019f-107">Prerequisites</span></span>
<span data-ttu-id="0019f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0019f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0019f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0019f-110">Permission type</span></span>|<span data-ttu-id="0019f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0019f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0019f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0019f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0019f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0019f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0019f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0019f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0019f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0019f-115">Not supported.</span></span>|
|<span data-ttu-id="0019f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0019f-116">Application</span></span>|<span data-ttu-id="0019f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0019f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0019f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0019f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0019f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0019f-119">Request headers</span></span>
|<span data-ttu-id="0019f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0019f-120">Header</span></span>|<span data-ttu-id="0019f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="0019f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0019f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0019f-122">Authorization</span></span>|<span data-ttu-id="0019f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0019f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0019f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0019f-124">Accept</span></span>|<span data-ttu-id="0019f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0019f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0019f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0019f-126">Request body</span></span>
<span data-ttu-id="0019f-127">No corpo da solicitação, forneça uma representação JSON do objeto officeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="0019f-127">In the request body, supply a JSON representation for the officeSuiteApp object.</span></span>

<span data-ttu-id="0019f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar officeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="0019f-128">The following table shows the properties that are required when you create the officeSuiteApp.</span></span>

|<span data-ttu-id="0019f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0019f-129">Property</span></span>|<span data-ttu-id="0019f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0019f-130">Type</span></span>|<span data-ttu-id="0019f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0019f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0019f-132">id</span><span class="sxs-lookup"><span data-stu-id="0019f-132">id</span></span>|<span data-ttu-id="0019f-133">String</span><span class="sxs-lookup"><span data-stu-id="0019f-133">String</span></span>|<span data-ttu-id="0019f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0019f-134">Key of the entity.</span></span> <span data-ttu-id="0019f-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0019f-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0019f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0019f-136">displayName</span></span>|<span data-ttu-id="0019f-137">String</span><span class="sxs-lookup"><span data-stu-id="0019f-137">String</span></span>|<span data-ttu-id="0019f-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="0019f-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0019f-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0019f-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0019f-140">descrição</span><span class="sxs-lookup"><span data-stu-id="0019f-140">description</span></span>|<span data-ttu-id="0019f-141">String</span><span class="sxs-lookup"><span data-stu-id="0019f-141">String</span></span>|<span data-ttu-id="0019f-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0019f-142">The description of the app.</span></span> <span data-ttu-id="0019f-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0019f-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0019f-144">publicador</span><span class="sxs-lookup"><span data-stu-id="0019f-144">publisher</span></span>|<span data-ttu-id="0019f-145">String</span><span class="sxs-lookup"><span data-stu-id="0019f-145">String</span></span>|<span data-ttu-id="0019f-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0019f-146">The publisher of the app.</span></span> <span data-ttu-id="0019f-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0019f-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0019f-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0019f-148">largeIcon</span></span>|[<span data-ttu-id="0019f-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0019f-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0019f-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="0019f-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0019f-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0019f-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0019f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0019f-152">createdDateTime</span></span>|<span data-ttu-id="0019f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0019f-153">DateTimeOffset</span></span>|<span data-ttu-id="0019f-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0019f-154">The date and time the app was created.</span></span> <span data-ttu-id="0019f-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0019f-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0019f-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0019f-156">lastModifiedDateTime</span></span>|<span data-ttu-id="0019f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0019f-157">DateTimeOffset</span></span>|<span data-ttu-id="0019f-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0019f-158">The date and time the app was last modified.</span></span> <span data-ttu-id="0019f-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0019f-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0019f-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0019f-160">isFeatured</span></span>|<span data-ttu-id="0019f-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="0019f-161">Boolean</span></span>|<span data-ttu-id="0019f-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0019f-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0019f-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0019f-163">privacyInformationUrl</span></span>|<span data-ttu-id="0019f-164">String</span><span class="sxs-lookup"><span data-stu-id="0019f-164">String</span></span>|<span data-ttu-id="0019f-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="0019f-165">The privacy statement Url.</span></span> <span data-ttu-id="0019f-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0019f-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0019f-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0019f-167">informationUrl</span></span>|<span data-ttu-id="0019f-168">String</span><span class="sxs-lookup"><span data-stu-id="0019f-168">String</span></span>|<span data-ttu-id="0019f-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="0019f-169">The more information Url.</span></span> <span data-ttu-id="0019f-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0019f-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0019f-171">owner</span><span class="sxs-lookup"><span data-stu-id="0019f-171">owner</span></span>|<span data-ttu-id="0019f-172">String</span><span class="sxs-lookup"><span data-stu-id="0019f-172">String</span></span>|<span data-ttu-id="0019f-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="0019f-173">The owner of the app.</span></span> <span data-ttu-id="0019f-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0019f-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0019f-175">developer</span><span class="sxs-lookup"><span data-stu-id="0019f-175">developer</span></span>|<span data-ttu-id="0019f-176">String</span><span class="sxs-lookup"><span data-stu-id="0019f-176">String</span></span>|<span data-ttu-id="0019f-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0019f-177">The developer of the app.</span></span> <span data-ttu-id="0019f-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0019f-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0019f-179">notes</span><span class="sxs-lookup"><span data-stu-id="0019f-179">notes</span></span>|<span data-ttu-id="0019f-180">String</span><span class="sxs-lookup"><span data-stu-id="0019f-180">String</span></span>|<span data-ttu-id="0019f-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0019f-181">Notes for the app.</span></span> <span data-ttu-id="0019f-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0019f-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0019f-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="0019f-183">uploadState</span></span>|<span data-ttu-id="0019f-184">Int32</span><span class="sxs-lookup"><span data-stu-id="0019f-184">Int32</span></span>|<span data-ttu-id="0019f-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="0019f-185">The upload state.</span></span> <span data-ttu-id="0019f-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0019f-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0019f-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="0019f-187">publishingState</span></span>|[<span data-ttu-id="0019f-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0019f-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0019f-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0019f-189">The publishing state for the app.</span></span> <span data-ttu-id="0019f-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="0019f-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0019f-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0019f-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="0019f-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0019f-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0019f-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="0019f-193">isAssigned</span></span>|<span data-ttu-id="0019f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="0019f-194">Boolean</span></span>|<span data-ttu-id="0019f-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="0019f-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="0019f-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0019f-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0019f-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0019f-197">roleScopeTagIds</span></span>|<span data-ttu-id="0019f-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0019f-198">String collection</span></span>|<span data-ttu-id="0019f-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="0019f-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="0019f-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0019f-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0019f-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="0019f-201">dependentAppCount</span></span>|<span data-ttu-id="0019f-202">Int32</span><span class="sxs-lookup"><span data-stu-id="0019f-202">Int32</span></span>|<span data-ttu-id="0019f-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="0019f-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="0019f-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0019f-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0019f-205">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="0019f-205">autoAcceptEula</span></span>|<span data-ttu-id="0019f-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="0019f-206">Boolean</span></span>|<span data-ttu-id="0019f-207">O valor para aceitar o EULA automaticamente no dispositivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="0019f-207">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="0019f-208">productIds</span><span class="sxs-lookup"><span data-stu-id="0019f-208">productIds</span></span>|<span data-ttu-id="0019f-209">coleção [officeProductId](../resources/intune-apps-officeproductid.md)</span><span class="sxs-lookup"><span data-stu-id="0019f-209">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="0019f-210">As IDs de produto que representam a SKU do pacote do office365.</span><span class="sxs-lookup"><span data-stu-id="0019f-210">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="0019f-211">Os valores possíveis são: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span><span class="sxs-lookup"><span data-stu-id="0019f-211">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="0019f-212">excludedApps</span><span class="sxs-lookup"><span data-stu-id="0019f-212">excludedApps</span></span>|[<span data-ttu-id="0019f-213">excludedApps</span><span class="sxs-lookup"><span data-stu-id="0019f-213">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="0019f-214">A propriedade para representar os aplicativos que são excluídos da ID de produto do Office365 selecionado.</span><span class="sxs-lookup"><span data-stu-id="0019f-214">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="0019f-215">Propriedades usesharedcomputeractivation</span><span class="sxs-lookup"><span data-stu-id="0019f-215">useSharedComputerActivation</span></span>|<span data-ttu-id="0019f-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="0019f-216">Boolean</span></span>|<span data-ttu-id="0019f-217">A propriedade que representa se a ativação de computador compartilhado é usada não para o pacote de aplicativos do office365.</span><span class="sxs-lookup"><span data-stu-id="0019f-217">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="0019f-218">updateChannel</span><span class="sxs-lookup"><span data-stu-id="0019f-218">updateChannel</span></span>|[<span data-ttu-id="0019f-219">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="0019f-219">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="0019f-220">A propriedade para representar o canal de atualização do office365.</span><span class="sxs-lookup"><span data-stu-id="0019f-220">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="0019f-221">Os valores possíveis são: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span><span class="sxs-lookup"><span data-stu-id="0019f-221">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="0019f-222">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="0019f-222">officePlatformArchitecture</span></span>|[<span data-ttu-id="0019f-223">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="0019f-223">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="0019f-224">A propriedade para representar a versão do pacote de aplicativos do office365.</span><span class="sxs-lookup"><span data-stu-id="0019f-224">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="0019f-225">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="0019f-225">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="0019f-226">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="0019f-226">localesToInstall</span></span>|<span data-ttu-id="0019f-227">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0019f-227">String collection</span></span>|<span data-ttu-id="0019f-228">A propriedade para representar os locais que são instalados quando os aplicativos do Office365 estão instalados.</span><span class="sxs-lookup"><span data-stu-id="0019f-228">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="0019f-229">Ele usa RFC 6033 padrão.</span><span class="sxs-lookup"><span data-stu-id="0019f-229">It uses standard RFC 6033.</span></span> <span data-ttu-id="0019f-230">Refhttps://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="0019f-230">Ref: https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="0019f-231">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="0019f-231">installProgressDisplayLevel</span></span>|[<span data-ttu-id="0019f-232">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="0019f-232">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="0019f-233">Para especificar o nível de exibição da interface do usuário da configuração de progresso da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0019f-233">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="0019f-234">Os valores possíveis são: `none` e `full`.</span><span class="sxs-lookup"><span data-stu-id="0019f-234">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="0019f-235">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="0019f-235">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="0019f-236">Booliano</span><span class="sxs-lookup"><span data-stu-id="0019f-236">Boolean</span></span>|<span data-ttu-id="0019f-237">A propriedade para determinar se deve desinstalar o Office MSI existente se um pacote de aplicativos do Office365 for implantado no dispositivo ou não.</span><span class="sxs-lookup"><span data-stu-id="0019f-237">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="0019f-238">targetVersion</span><span class="sxs-lookup"><span data-stu-id="0019f-238">targetVersion</span></span>|<span data-ttu-id="0019f-239">String</span><span class="sxs-lookup"><span data-stu-id="0019f-239">String</span></span>|<span data-ttu-id="0019f-240">A propriedade para representar a versão de destino específica para o pacote de aplicativos do Office365 que deve permanecer implantado nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="0019f-240">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="0019f-241">updateVersion</span><span class="sxs-lookup"><span data-stu-id="0019f-241">updateVersion</span></span>|<span data-ttu-id="0019f-242">String</span><span class="sxs-lookup"><span data-stu-id="0019f-242">String</span></span>|<span data-ttu-id="0019f-243">A propriedade para representar a versão de atualização na qual a versão de destino específica está disponível para o pacote de aplicativos do office365.</span><span class="sxs-lookup"><span data-stu-id="0019f-243">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="0019f-244">officeConfigurationXml</span><span class="sxs-lookup"><span data-stu-id="0019f-244">officeConfigurationXml</span></span>|<span data-ttu-id="0019f-245">Binária</span><span class="sxs-lookup"><span data-stu-id="0019f-245">Binary</span></span>|<span data-ttu-id="0019f-246">A propriedade para representar o arquivo de configuração XML que pode ser especificado para aplicativos do Office ProPlus.</span><span class="sxs-lookup"><span data-stu-id="0019f-246">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="0019f-247">Tem precedência sobre todas as outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="0019f-247">Takes precedence over all other properties.</span></span> <span data-ttu-id="0019f-248">Quando presente, o arquivo de configuração XML será usado para criar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0019f-248">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="0019f-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="0019f-249">Response</span></span>
<span data-ttu-id="0019f-250">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0019f-250">If successful, this method returns a `201 Created` response code and a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0019f-251">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0019f-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="0019f-252">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0019f-252">Request</span></span>
<span data-ttu-id="0019f-253">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0019f-253">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="0019f-254">Resposta</span><span class="sxs-lookup"><span data-stu-id="0019f-254">Response</span></span>
<span data-ttu-id="0019f-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0019f-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





