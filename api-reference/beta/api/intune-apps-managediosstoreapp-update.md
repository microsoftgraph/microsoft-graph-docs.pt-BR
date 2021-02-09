---
title: Atualizar managedIOSStoreApp
description: Atualiza as propriedades de um objeto managedIOSStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 63eb9a6a421540f198124914f7603afbf97afc17
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155402"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="4fab3-103">Atualizar managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="4fab3-103">Update managedIOSStoreApp</span></span>

<span data-ttu-id="4fab3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fab3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4fab3-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4fab3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fab3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4fab3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fab3-107">Atualiza as propriedades de um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="4fab3-107">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fab3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4fab3-108">Prerequisites</span></span>
<span data-ttu-id="4fab3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fab3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fab3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4fab3-111">Permission type</span></span>|<span data-ttu-id="4fab3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4fab3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fab3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4fab3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4fab3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fab3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4fab3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4fab3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fab3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4fab3-116">Not supported.</span></span>|
|<span data-ttu-id="4fab3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4fab3-117">Application</span></span>|<span data-ttu-id="4fab3-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fab3-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fab3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4fab3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="4fab3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4fab3-120">Request headers</span></span>
|<span data-ttu-id="4fab3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4fab3-121">Header</span></span>|<span data-ttu-id="4fab3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4fab3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fab3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4fab3-123">Authorization</span></span>|<span data-ttu-id="4fab3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4fab3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fab3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4fab3-125">Accept</span></span>|<span data-ttu-id="4fab3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4fab3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fab3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4fab3-127">Request body</span></span>
<span data-ttu-id="4fab3-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="4fab3-128">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="4fab3-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="4fab3-129">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="4fab3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4fab3-130">Property</span></span>|<span data-ttu-id="4fab3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4fab3-131">Type</span></span>|<span data-ttu-id="4fab3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fab3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fab3-133">id</span><span class="sxs-lookup"><span data-stu-id="4fab3-133">id</span></span>|<span data-ttu-id="4fab3-134">String</span><span class="sxs-lookup"><span data-stu-id="4fab3-134">String</span></span>|<span data-ttu-id="4fab3-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4fab3-135">Key of the entity.</span></span> <span data-ttu-id="4fab3-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4fab3-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4fab3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4fab3-137">displayName</span></span>|<span data-ttu-id="4fab3-138">String</span><span class="sxs-lookup"><span data-stu-id="4fab3-138">String</span></span>|<span data-ttu-id="4fab3-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="4fab3-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4fab3-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4fab3-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4fab3-141">description</span><span class="sxs-lookup"><span data-stu-id="4fab3-141">description</span></span>|<span data-ttu-id="4fab3-142">String</span><span class="sxs-lookup"><span data-stu-id="4fab3-142">String</span></span>|<span data-ttu-id="4fab3-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4fab3-143">The description of the app.</span></span> <span data-ttu-id="4fab3-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4fab3-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4fab3-145">publicador</span><span class="sxs-lookup"><span data-stu-id="4fab3-145">publisher</span></span>|<span data-ttu-id="4fab3-146">String</span><span class="sxs-lookup"><span data-stu-id="4fab3-146">String</span></span>|<span data-ttu-id="4fab3-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4fab3-147">The publisher of the app.</span></span> <span data-ttu-id="4fab3-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4fab3-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4fab3-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4fab3-149">largeIcon</span></span>|[<span data-ttu-id="4fab3-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4fab3-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4fab3-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="4fab3-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4fab3-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4fab3-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4fab3-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4fab3-153">createdDateTime</span></span>|<span data-ttu-id="4fab3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fab3-154">DateTimeOffset</span></span>|<span data-ttu-id="4fab3-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4fab3-155">The date and time the app was created.</span></span> <span data-ttu-id="4fab3-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4fab3-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4fab3-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4fab3-157">lastModifiedDateTime</span></span>|<span data-ttu-id="4fab3-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fab3-158">DateTimeOffset</span></span>|<span data-ttu-id="4fab3-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4fab3-159">The date and time the app was last modified.</span></span> <span data-ttu-id="4fab3-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4fab3-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4fab3-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4fab3-161">isFeatured</span></span>|<span data-ttu-id="4fab3-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fab3-162">Boolean</span></span>|<span data-ttu-id="4fab3-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4fab3-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4fab3-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4fab3-164">privacyInformationUrl</span></span>|<span data-ttu-id="4fab3-165">String</span><span class="sxs-lookup"><span data-stu-id="4fab3-165">String</span></span>|<span data-ttu-id="4fab3-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="4fab3-166">The privacy statement Url.</span></span> <span data-ttu-id="4fab3-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4fab3-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4fab3-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4fab3-168">informationUrl</span></span>|<span data-ttu-id="4fab3-169">String</span><span class="sxs-lookup"><span data-stu-id="4fab3-169">String</span></span>|<span data-ttu-id="4fab3-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="4fab3-170">The more information Url.</span></span> <span data-ttu-id="4fab3-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4fab3-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4fab3-172">owner</span><span class="sxs-lookup"><span data-stu-id="4fab3-172">owner</span></span>|<span data-ttu-id="4fab3-173">String</span><span class="sxs-lookup"><span data-stu-id="4fab3-173">String</span></span>|<span data-ttu-id="4fab3-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4fab3-174">The owner of the app.</span></span> <span data-ttu-id="4fab3-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4fab3-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4fab3-176">developer</span><span class="sxs-lookup"><span data-stu-id="4fab3-176">developer</span></span>|<span data-ttu-id="4fab3-177">String</span><span class="sxs-lookup"><span data-stu-id="4fab3-177">String</span></span>|<span data-ttu-id="4fab3-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4fab3-178">The developer of the app.</span></span> <span data-ttu-id="4fab3-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4fab3-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4fab3-180">notes</span><span class="sxs-lookup"><span data-stu-id="4fab3-180">notes</span></span>|<span data-ttu-id="4fab3-181">String</span><span class="sxs-lookup"><span data-stu-id="4fab3-181">String</span></span>|<span data-ttu-id="4fab3-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4fab3-182">Notes for the app.</span></span> <span data-ttu-id="4fab3-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4fab3-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4fab3-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="4fab3-184">uploadState</span></span>|<span data-ttu-id="4fab3-185">Int32</span><span class="sxs-lookup"><span data-stu-id="4fab3-185">Int32</span></span>|<span data-ttu-id="4fab3-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="4fab3-186">The upload state.</span></span> <span data-ttu-id="4fab3-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="4fab3-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="4fab3-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4fab3-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4fab3-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="4fab3-189">publishingState</span></span>|[<span data-ttu-id="4fab3-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4fab3-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4fab3-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4fab3-191">The publishing state for the app.</span></span> <span data-ttu-id="4fab3-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="4fab3-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4fab3-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4fab3-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="4fab3-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4fab3-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4fab3-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4fab3-195">isAssigned</span></span>|<span data-ttu-id="4fab3-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fab3-196">Boolean</span></span>|<span data-ttu-id="4fab3-197">O valor que indica se o aplicativo está atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="4fab3-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4fab3-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4fab3-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4fab3-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4fab3-199">roleScopeTagIds</span></span>|<span data-ttu-id="4fab3-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4fab3-200">String collection</span></span>|<span data-ttu-id="4fab3-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="4fab3-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4fab3-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4fab3-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4fab3-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="4fab3-203">dependentAppCount</span></span>|<span data-ttu-id="4fab3-204">Int32</span><span class="sxs-lookup"><span data-stu-id="4fab3-204">Int32</span></span>|<span data-ttu-id="4fab3-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="4fab3-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="4fab3-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4fab3-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4fab3-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="4fab3-207">supersedingAppCount</span></span>|<span data-ttu-id="4fab3-208">Int32</span><span class="sxs-lookup"><span data-stu-id="4fab3-208">Int32</span></span>|<span data-ttu-id="4fab3-209">O número total de aplicativos que este aplicativo é direta ou indiretamente é supersedido.</span><span class="sxs-lookup"><span data-stu-id="4fab3-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="4fab3-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4fab3-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4fab3-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="4fab3-211">supersededAppCount</span></span>|<span data-ttu-id="4fab3-212">Int32</span><span class="sxs-lookup"><span data-stu-id="4fab3-212">Int32</span></span>|<span data-ttu-id="4fab3-213">O número total de aplicativos pelos quais esse aplicativo é direta ou indiretamente sobressu valorado.</span><span class="sxs-lookup"><span data-stu-id="4fab3-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="4fab3-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4fab3-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4fab3-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="4fab3-215">appAvailability</span></span>|[<span data-ttu-id="4fab3-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="4fab3-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="4fab3-217">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4fab3-217">The Application's availability.</span></span> <span data-ttu-id="4fab3-218">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="4fab3-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="4fab3-219">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="4fab3-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="4fab3-220">version</span><span class="sxs-lookup"><span data-stu-id="4fab3-220">version</span></span>|<span data-ttu-id="4fab3-221">String</span><span class="sxs-lookup"><span data-stu-id="4fab3-221">String</span></span>|<span data-ttu-id="4fab3-222">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4fab3-222">The Application's version.</span></span> <span data-ttu-id="4fab3-223">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="4fab3-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="4fab3-224">bundleId</span><span class="sxs-lookup"><span data-stu-id="4fab3-224">bundleId</span></span>|<span data-ttu-id="4fab3-225">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4fab3-225">String</span></span>|<span data-ttu-id="4fab3-226">A ID do pacote de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="4fab3-226">The app's Bundle ID.</span></span>|
|<span data-ttu-id="4fab3-227">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="4fab3-227">appStoreUrl</span></span>|<span data-ttu-id="4fab3-228">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4fab3-228">String</span></span>|<span data-ttu-id="4fab3-229">A AppStoreUrl da Apple.</span><span class="sxs-lookup"><span data-stu-id="4fab3-229">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="4fab3-230">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="4fab3-230">applicableDeviceType</span></span>|[<span data-ttu-id="4fab3-231">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="4fab3-231">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="4fab3-232">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="4fab3-232">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="4fab3-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4fab3-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4fab3-234">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4fab3-234">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="4fab3-235">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="4fab3-235">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="4fab3-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fab3-236">Response</span></span>
<span data-ttu-id="4fab3-237">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4fab3-237">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fab3-238">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4fab3-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fab3-239">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4fab3-239">Request</span></span>
<span data-ttu-id="4fab3-240">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4fab3-240">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1315

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true,
    "v14_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="4fab3-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="4fab3-241">Response</span></span>
<span data-ttu-id="4fab3-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4fab3-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1487

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true,
    "v14_0": true
  }
}
```




