---
title: Atualizar managedAndroidStoreApp
description: Atualiza as propriedades de um objeto managedAndroidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3a0a0da927569ce33e7d26d46442a5caed9350de
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155458"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="f2a51-103">Atualizar managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="f2a51-103">Update managedAndroidStoreApp</span></span>

<span data-ttu-id="f2a51-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2a51-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2a51-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f2a51-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2a51-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2a51-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2a51-107">Atualiza as propriedades de um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2a51-107">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2a51-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2a51-108">Prerequisites</span></span>
<span data-ttu-id="f2a51-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2a51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2a51-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2a51-111">Permission type</span></span>|<span data-ttu-id="f2a51-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2a51-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2a51-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2a51-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2a51-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2a51-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f2a51-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2a51-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2a51-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2a51-116">Not supported.</span></span>|
|<span data-ttu-id="f2a51-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2a51-117">Application</span></span>|<span data-ttu-id="f2a51-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2a51-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2a51-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2a51-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f2a51-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2a51-120">Request headers</span></span>
|<span data-ttu-id="f2a51-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2a51-121">Header</span></span>|<span data-ttu-id="f2a51-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f2a51-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2a51-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2a51-123">Authorization</span></span>|<span data-ttu-id="f2a51-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2a51-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2a51-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2a51-125">Accept</span></span>|<span data-ttu-id="f2a51-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2a51-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2a51-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2a51-127">Request body</span></span>
<span data-ttu-id="f2a51-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2a51-128">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="f2a51-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2a51-129">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="f2a51-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2a51-130">Property</span></span>|<span data-ttu-id="f2a51-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2a51-131">Type</span></span>|<span data-ttu-id="f2a51-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2a51-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2a51-133">id</span><span class="sxs-lookup"><span data-stu-id="f2a51-133">id</span></span>|<span data-ttu-id="f2a51-134">String</span><span class="sxs-lookup"><span data-stu-id="f2a51-134">String</span></span>|<span data-ttu-id="f2a51-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f2a51-135">Key of the entity.</span></span> <span data-ttu-id="f2a51-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a51-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a51-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f2a51-137">displayName</span></span>|<span data-ttu-id="f2a51-138">String</span><span class="sxs-lookup"><span data-stu-id="f2a51-138">String</span></span>|<span data-ttu-id="f2a51-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f2a51-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f2a51-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a51-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a51-141">description</span><span class="sxs-lookup"><span data-stu-id="f2a51-141">description</span></span>|<span data-ttu-id="f2a51-142">String</span><span class="sxs-lookup"><span data-stu-id="f2a51-142">String</span></span>|<span data-ttu-id="f2a51-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2a51-143">The description of the app.</span></span> <span data-ttu-id="f2a51-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a51-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a51-145">publicador</span><span class="sxs-lookup"><span data-stu-id="f2a51-145">publisher</span></span>|<span data-ttu-id="f2a51-146">String</span><span class="sxs-lookup"><span data-stu-id="f2a51-146">String</span></span>|<span data-ttu-id="f2a51-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2a51-147">The publisher of the app.</span></span> <span data-ttu-id="f2a51-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a51-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a51-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f2a51-149">largeIcon</span></span>|[<span data-ttu-id="f2a51-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f2a51-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f2a51-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="f2a51-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f2a51-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a51-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a51-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2a51-153">createdDateTime</span></span>|<span data-ttu-id="f2a51-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2a51-154">DateTimeOffset</span></span>|<span data-ttu-id="f2a51-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2a51-155">The date and time the app was created.</span></span> <span data-ttu-id="f2a51-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a51-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a51-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2a51-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f2a51-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2a51-158">DateTimeOffset</span></span>|<span data-ttu-id="f2a51-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f2a51-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f2a51-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a51-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a51-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f2a51-161">isFeatured</span></span>|<span data-ttu-id="f2a51-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2a51-162">Boolean</span></span>|<span data-ttu-id="f2a51-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a51-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a51-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f2a51-164">privacyInformationUrl</span></span>|<span data-ttu-id="f2a51-165">String</span><span class="sxs-lookup"><span data-stu-id="f2a51-165">String</span></span>|<span data-ttu-id="f2a51-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="f2a51-166">The privacy statement Url.</span></span> <span data-ttu-id="f2a51-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a51-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a51-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f2a51-168">informationUrl</span></span>|<span data-ttu-id="f2a51-169">String</span><span class="sxs-lookup"><span data-stu-id="f2a51-169">String</span></span>|<span data-ttu-id="f2a51-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="f2a51-170">The more information Url.</span></span> <span data-ttu-id="f2a51-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a51-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a51-172">owner</span><span class="sxs-lookup"><span data-stu-id="f2a51-172">owner</span></span>|<span data-ttu-id="f2a51-173">String</span><span class="sxs-lookup"><span data-stu-id="f2a51-173">String</span></span>|<span data-ttu-id="f2a51-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f2a51-174">The owner of the app.</span></span> <span data-ttu-id="f2a51-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a51-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a51-176">developer</span><span class="sxs-lookup"><span data-stu-id="f2a51-176">developer</span></span>|<span data-ttu-id="f2a51-177">String</span><span class="sxs-lookup"><span data-stu-id="f2a51-177">String</span></span>|<span data-ttu-id="f2a51-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2a51-178">The developer of the app.</span></span> <span data-ttu-id="f2a51-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a51-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a51-180">notes</span><span class="sxs-lookup"><span data-stu-id="f2a51-180">notes</span></span>|<span data-ttu-id="f2a51-181">String</span><span class="sxs-lookup"><span data-stu-id="f2a51-181">String</span></span>|<span data-ttu-id="f2a51-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2a51-182">Notes for the app.</span></span> <span data-ttu-id="f2a51-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a51-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a51-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f2a51-184">uploadState</span></span>|<span data-ttu-id="f2a51-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f2a51-185">Int32</span></span>|<span data-ttu-id="f2a51-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="f2a51-186">The upload state.</span></span> <span data-ttu-id="f2a51-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="f2a51-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="f2a51-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a51-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a51-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="f2a51-189">publishingState</span></span>|[<span data-ttu-id="f2a51-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f2a51-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f2a51-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2a51-191">The publishing state for the app.</span></span> <span data-ttu-id="f2a51-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="f2a51-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f2a51-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2a51-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="f2a51-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f2a51-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f2a51-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f2a51-195">isAssigned</span></span>|<span data-ttu-id="f2a51-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2a51-196">Boolean</span></span>|<span data-ttu-id="f2a51-197">O valor que indica se o aplicativo está atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="f2a51-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f2a51-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a51-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a51-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f2a51-199">roleScopeTagIds</span></span>|<span data-ttu-id="f2a51-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2a51-200">String collection</span></span>|<span data-ttu-id="f2a51-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="f2a51-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f2a51-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a51-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a51-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="f2a51-203">dependentAppCount</span></span>|<span data-ttu-id="f2a51-204">Int32</span><span class="sxs-lookup"><span data-stu-id="f2a51-204">Int32</span></span>|<span data-ttu-id="f2a51-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="f2a51-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="f2a51-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a51-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a51-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="f2a51-207">supersedingAppCount</span></span>|<span data-ttu-id="f2a51-208">Int32</span><span class="sxs-lookup"><span data-stu-id="f2a51-208">Int32</span></span>|<span data-ttu-id="f2a51-209">O número total de aplicativos que este aplicativo é direta ou indiretamente é supersedido.</span><span class="sxs-lookup"><span data-stu-id="f2a51-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="f2a51-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a51-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a51-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="f2a51-211">supersededAppCount</span></span>|<span data-ttu-id="f2a51-212">Int32</span><span class="sxs-lookup"><span data-stu-id="f2a51-212">Int32</span></span>|<span data-ttu-id="f2a51-213">O número total de aplicativos pelos quais esse aplicativo é direta ou indiretamente sobressu valorado.</span><span class="sxs-lookup"><span data-stu-id="f2a51-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="f2a51-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a51-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a51-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="f2a51-215">appAvailability</span></span>|[<span data-ttu-id="f2a51-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="f2a51-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="f2a51-217">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2a51-217">The Application's availability.</span></span> <span data-ttu-id="f2a51-218">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2a51-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="f2a51-219">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="f2a51-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="f2a51-220">version</span><span class="sxs-lookup"><span data-stu-id="f2a51-220">version</span></span>|<span data-ttu-id="f2a51-221">String</span><span class="sxs-lookup"><span data-stu-id="f2a51-221">String</span></span>|<span data-ttu-id="f2a51-222">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2a51-222">The Application's version.</span></span> <span data-ttu-id="f2a51-223">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2a51-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="f2a51-224">packageId</span><span class="sxs-lookup"><span data-stu-id="f2a51-224">packageId</span></span>|<span data-ttu-id="f2a51-225">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2a51-225">String</span></span>|<span data-ttu-id="f2a51-226">A ID de pacote do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2a51-226">The app's package ID.</span></span>|
|<span data-ttu-id="f2a51-227">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f2a51-227">appStoreUrl</span></span>|<span data-ttu-id="f2a51-228">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2a51-228">String</span></span>|<span data-ttu-id="f2a51-229">A AppStoreUrl do Android.</span><span class="sxs-lookup"><span data-stu-id="f2a51-229">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="f2a51-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f2a51-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f2a51-231">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f2a51-231">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="f2a51-232">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="f2a51-232">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="f2a51-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2a51-233">Response</span></span>
<span data-ttu-id="f2a51-234">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2a51-234">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2a51-235">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2a51-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2a51-236">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2a51-236">Request</span></span>
<span data-ttu-id="f2a51-237">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2a51-237">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1361

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="f2a51-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2a51-238">Response</span></span>
<span data-ttu-id="f2a51-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2a51-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1533

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  }
}
```




