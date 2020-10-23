---
title: Criar officeSuiteApp
description: Criar um novo objeto officeSuiteApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 35ac41caf7504c6b2754103b9fb16891eb515a48
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723676"
---
# <a name="create-officesuiteapp"></a><span data-ttu-id="e79dd-103">Criar officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="e79dd-103">Create officeSuiteApp</span></span>

<span data-ttu-id="e79dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e79dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e79dd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e79dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e79dd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e79dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e79dd-107">Criar um novo objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e79dd-107">Create a new [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e79dd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e79dd-108">Prerequisites</span></span>
<span data-ttu-id="e79dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e79dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e79dd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e79dd-111">Permission type</span></span>|<span data-ttu-id="e79dd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e79dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e79dd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e79dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e79dd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e79dd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e79dd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e79dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e79dd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e79dd-116">Not supported.</span></span>|
|<span data-ttu-id="e79dd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e79dd-117">Application</span></span>|<span data-ttu-id="e79dd-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e79dd-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e79dd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e79dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e79dd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e79dd-120">Request headers</span></span>
|<span data-ttu-id="e79dd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e79dd-121">Header</span></span>|<span data-ttu-id="e79dd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e79dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e79dd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e79dd-123">Authorization</span></span>|<span data-ttu-id="e79dd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e79dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e79dd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e79dd-125">Accept</span></span>|<span data-ttu-id="e79dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e79dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e79dd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e79dd-127">Request body</span></span>
<span data-ttu-id="e79dd-128">No corpo da solicitação, forneça uma representação JSON do objeto officeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="e79dd-128">In the request body, supply a JSON representation for the officeSuiteApp object.</span></span>

<span data-ttu-id="e79dd-129">A tabela a seguir mostra as propriedades que são necessárias ao criar officeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="e79dd-129">The following table shows the properties that are required when you create the officeSuiteApp.</span></span>

|<span data-ttu-id="e79dd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e79dd-130">Property</span></span>|<span data-ttu-id="e79dd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e79dd-131">Type</span></span>|<span data-ttu-id="e79dd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e79dd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e79dd-133">id</span><span class="sxs-lookup"><span data-stu-id="e79dd-133">id</span></span>|<span data-ttu-id="e79dd-134">String</span><span class="sxs-lookup"><span data-stu-id="e79dd-134">String</span></span>|<span data-ttu-id="e79dd-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e79dd-135">Key of the entity.</span></span> <span data-ttu-id="e79dd-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e79dd-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e79dd-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e79dd-137">displayName</span></span>|<span data-ttu-id="e79dd-138">String</span><span class="sxs-lookup"><span data-stu-id="e79dd-138">String</span></span>|<span data-ttu-id="e79dd-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="e79dd-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e79dd-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e79dd-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e79dd-141">description</span><span class="sxs-lookup"><span data-stu-id="e79dd-141">description</span></span>|<span data-ttu-id="e79dd-142">String</span><span class="sxs-lookup"><span data-stu-id="e79dd-142">String</span></span>|<span data-ttu-id="e79dd-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e79dd-143">The description of the app.</span></span> <span data-ttu-id="e79dd-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e79dd-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e79dd-145">publicador</span><span class="sxs-lookup"><span data-stu-id="e79dd-145">publisher</span></span>|<span data-ttu-id="e79dd-146">String</span><span class="sxs-lookup"><span data-stu-id="e79dd-146">String</span></span>|<span data-ttu-id="e79dd-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e79dd-147">The publisher of the app.</span></span> <span data-ttu-id="e79dd-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e79dd-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e79dd-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e79dd-149">largeIcon</span></span>|[<span data-ttu-id="e79dd-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e79dd-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e79dd-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="e79dd-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e79dd-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e79dd-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e79dd-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e79dd-153">createdDateTime</span></span>|<span data-ttu-id="e79dd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e79dd-154">DateTimeOffset</span></span>|<span data-ttu-id="e79dd-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e79dd-155">The date and time the app was created.</span></span> <span data-ttu-id="e79dd-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e79dd-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e79dd-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e79dd-157">lastModifiedDateTime</span></span>|<span data-ttu-id="e79dd-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e79dd-158">DateTimeOffset</span></span>|<span data-ttu-id="e79dd-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e79dd-159">The date and time the app was last modified.</span></span> <span data-ttu-id="e79dd-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e79dd-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e79dd-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e79dd-161">isFeatured</span></span>|<span data-ttu-id="e79dd-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e79dd-162">Boolean</span></span>|<span data-ttu-id="e79dd-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e79dd-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e79dd-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e79dd-164">privacyInformationUrl</span></span>|<span data-ttu-id="e79dd-165">String</span><span class="sxs-lookup"><span data-stu-id="e79dd-165">String</span></span>|<span data-ttu-id="e79dd-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="e79dd-166">The privacy statement Url.</span></span> <span data-ttu-id="e79dd-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e79dd-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e79dd-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e79dd-168">informationUrl</span></span>|<span data-ttu-id="e79dd-169">String</span><span class="sxs-lookup"><span data-stu-id="e79dd-169">String</span></span>|<span data-ttu-id="e79dd-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="e79dd-170">The more information Url.</span></span> <span data-ttu-id="e79dd-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e79dd-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e79dd-172">owner</span><span class="sxs-lookup"><span data-stu-id="e79dd-172">owner</span></span>|<span data-ttu-id="e79dd-173">String</span><span class="sxs-lookup"><span data-stu-id="e79dd-173">String</span></span>|<span data-ttu-id="e79dd-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e79dd-174">The owner of the app.</span></span> <span data-ttu-id="e79dd-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e79dd-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e79dd-176">developer</span><span class="sxs-lookup"><span data-stu-id="e79dd-176">developer</span></span>|<span data-ttu-id="e79dd-177">String</span><span class="sxs-lookup"><span data-stu-id="e79dd-177">String</span></span>|<span data-ttu-id="e79dd-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e79dd-178">The developer of the app.</span></span> <span data-ttu-id="e79dd-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e79dd-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e79dd-180">notes</span><span class="sxs-lookup"><span data-stu-id="e79dd-180">notes</span></span>|<span data-ttu-id="e79dd-181">String</span><span class="sxs-lookup"><span data-stu-id="e79dd-181">String</span></span>|<span data-ttu-id="e79dd-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e79dd-182">Notes for the app.</span></span> <span data-ttu-id="e79dd-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e79dd-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e79dd-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="e79dd-184">uploadState</span></span>|<span data-ttu-id="e79dd-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e79dd-185">Int32</span></span>|<span data-ttu-id="e79dd-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="e79dd-186">The upload state.</span></span> <span data-ttu-id="e79dd-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="e79dd-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="e79dd-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e79dd-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e79dd-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="e79dd-189">publishingState</span></span>|[<span data-ttu-id="e79dd-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e79dd-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e79dd-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e79dd-191">The publishing state for the app.</span></span> <span data-ttu-id="e79dd-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="e79dd-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e79dd-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e79dd-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="e79dd-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e79dd-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e79dd-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e79dd-195">isAssigned</span></span>|<span data-ttu-id="e79dd-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="e79dd-196">Boolean</span></span>|<span data-ttu-id="e79dd-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="e79dd-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e79dd-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e79dd-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e79dd-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e79dd-199">roleScopeTagIds</span></span>|<span data-ttu-id="e79dd-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e79dd-200">String collection</span></span>|<span data-ttu-id="e79dd-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="e79dd-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e79dd-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e79dd-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e79dd-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="e79dd-203">dependentAppCount</span></span>|<span data-ttu-id="e79dd-204">Int32</span><span class="sxs-lookup"><span data-stu-id="e79dd-204">Int32</span></span>|<span data-ttu-id="e79dd-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="e79dd-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="e79dd-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e79dd-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e79dd-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="e79dd-207">supersedingAppCount</span></span>|<span data-ttu-id="e79dd-208">Int32</span><span class="sxs-lookup"><span data-stu-id="e79dd-208">Int32</span></span>|<span data-ttu-id="e79dd-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="e79dd-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="e79dd-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e79dd-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e79dd-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="e79dd-211">supersededAppCount</span></span>|<span data-ttu-id="e79dd-212">Int32</span><span class="sxs-lookup"><span data-stu-id="e79dd-212">Int32</span></span>|<span data-ttu-id="e79dd-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="e79dd-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="e79dd-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e79dd-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e79dd-215">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="e79dd-215">autoAcceptEula</span></span>|<span data-ttu-id="e79dd-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="e79dd-216">Boolean</span></span>|<span data-ttu-id="e79dd-217">O valor para aceitar o EULA automaticamente no dispositivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="e79dd-217">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="e79dd-218">productIds</span><span class="sxs-lookup"><span data-stu-id="e79dd-218">productIds</span></span>|<span data-ttu-id="e79dd-219">coleção [officeProductId](../resources/intune-apps-officeproductid.md)</span><span class="sxs-lookup"><span data-stu-id="e79dd-219">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="e79dd-220">As IDs de produto que representam a SKU do pacote do office365.</span><span class="sxs-lookup"><span data-stu-id="e79dd-220">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="e79dd-221">Os valores possíveis são: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span><span class="sxs-lookup"><span data-stu-id="e79dd-221">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="e79dd-222">excludedApps</span><span class="sxs-lookup"><span data-stu-id="e79dd-222">excludedApps</span></span>|[<span data-ttu-id="e79dd-223">excludedApps</span><span class="sxs-lookup"><span data-stu-id="e79dd-223">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="e79dd-224">A propriedade para representar os aplicativos que são excluídos da ID de produto do Office365 selecionado.</span><span class="sxs-lookup"><span data-stu-id="e79dd-224">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="e79dd-225">Propriedades usesharedcomputeractivation</span><span class="sxs-lookup"><span data-stu-id="e79dd-225">useSharedComputerActivation</span></span>|<span data-ttu-id="e79dd-226">Booliano</span><span class="sxs-lookup"><span data-stu-id="e79dd-226">Boolean</span></span>|<span data-ttu-id="e79dd-227">A propriedade que representa se a ativação de computador compartilhado é usada não para o pacote de aplicativos do office365.</span><span class="sxs-lookup"><span data-stu-id="e79dd-227">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="e79dd-228">updateChannel</span><span class="sxs-lookup"><span data-stu-id="e79dd-228">updateChannel</span></span>|[<span data-ttu-id="e79dd-229">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="e79dd-229">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="e79dd-230">A propriedade para representar o canal de atualização do office365.</span><span class="sxs-lookup"><span data-stu-id="e79dd-230">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="e79dd-231">Os possíveis valores são: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`, `monthlyEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="e79dd-231">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`, `monthlyEnterprise`.</span></span>|
|<span data-ttu-id="e79dd-232">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="e79dd-232">officePlatformArchitecture</span></span>|[<span data-ttu-id="e79dd-233">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="e79dd-233">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="e79dd-234">A propriedade para representar a versão do pacote de aplicativos do office365.</span><span class="sxs-lookup"><span data-stu-id="e79dd-234">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="e79dd-235">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="e79dd-235">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="e79dd-236">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="e79dd-236">localesToInstall</span></span>|<span data-ttu-id="e79dd-237">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e79dd-237">String collection</span></span>|<span data-ttu-id="e79dd-238">A propriedade para representar os locais que são instalados quando os aplicativos do Office365 estão instalados.</span><span class="sxs-lookup"><span data-stu-id="e79dd-238">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="e79dd-239">Ele usa RFC 6033 padrão.</span><span class="sxs-lookup"><span data-stu-id="e79dd-239">It uses standard RFC 6033.</span></span> <span data-ttu-id="e79dd-240">Ref https://technet.microsoft.com/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="e79dd-240">Ref: https://technet.microsoft.com/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="e79dd-241">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="e79dd-241">installProgressDisplayLevel</span></span>|[<span data-ttu-id="e79dd-242">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="e79dd-242">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="e79dd-243">Para especificar o nível de exibição da interface do usuário da configuração de progresso da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e79dd-243">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="e79dd-244">Os valores possíveis são: `none` e `full`.</span><span class="sxs-lookup"><span data-stu-id="e79dd-244">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="e79dd-245">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="e79dd-245">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="e79dd-246">Booliano</span><span class="sxs-lookup"><span data-stu-id="e79dd-246">Boolean</span></span>|<span data-ttu-id="e79dd-247">A propriedade para determinar se deve desinstalar o Office MSI existente se um pacote de aplicativos do Office365 for implantado no dispositivo ou não.</span><span class="sxs-lookup"><span data-stu-id="e79dd-247">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="e79dd-248">targetVersion</span><span class="sxs-lookup"><span data-stu-id="e79dd-248">targetVersion</span></span>|<span data-ttu-id="e79dd-249">String</span><span class="sxs-lookup"><span data-stu-id="e79dd-249">String</span></span>|<span data-ttu-id="e79dd-250">A propriedade para representar a versão de destino específica para o pacote de aplicativos do Office365 que deve permanecer implantado nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e79dd-250">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="e79dd-251">updateVersion</span><span class="sxs-lookup"><span data-stu-id="e79dd-251">updateVersion</span></span>|<span data-ttu-id="e79dd-252">String</span><span class="sxs-lookup"><span data-stu-id="e79dd-252">String</span></span>|<span data-ttu-id="e79dd-253">A propriedade para representar a versão de atualização na qual a versão de destino específica está disponível para o pacote de aplicativos do office365.</span><span class="sxs-lookup"><span data-stu-id="e79dd-253">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="e79dd-254">officeConfigurationXml</span><span class="sxs-lookup"><span data-stu-id="e79dd-254">officeConfigurationXml</span></span>|<span data-ttu-id="e79dd-255">Binária</span><span class="sxs-lookup"><span data-stu-id="e79dd-255">Binary</span></span>|<span data-ttu-id="e79dd-256">A propriedade para representar o arquivo de configuração XML que pode ser especificado para aplicativos do Office ProPlus.</span><span class="sxs-lookup"><span data-stu-id="e79dd-256">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="e79dd-257">Tem precedência sobre todas as outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="e79dd-257">Takes precedence over all other properties.</span></span> <span data-ttu-id="e79dd-258">Quando presente, o arquivo de configuração XML será usado para criar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e79dd-258">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="e79dd-259">Resposta</span><span class="sxs-lookup"><span data-stu-id="e79dd-259">Response</span></span>
<span data-ttu-id="e79dd-260">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e79dd-260">If successful, this method returns a `201 Created` response code and a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e79dd-261">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e79dd-261">Example</span></span>

### <a name="request"></a><span data-ttu-id="e79dd-262">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e79dd-262">Request</span></span>
<span data-ttu-id="e79dd-263">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e79dd-263">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="e79dd-264">Resposta</span><span class="sxs-lookup"><span data-stu-id="e79dd-264">Response</span></span>
<span data-ttu-id="e79dd-p127">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e79dd-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





