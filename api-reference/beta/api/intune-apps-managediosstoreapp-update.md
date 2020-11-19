---
title: Atualizar managedIOSStoreApp
description: Atualiza as propriedades de um objeto managedIOSStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ccf7bd5a7e6d8710e743a9b31287e4e0a2c5ea50
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49249649"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="50bce-103">Atualizar managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="50bce-103">Update managedIOSStoreApp</span></span>

<span data-ttu-id="50bce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50bce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50bce-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="50bce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50bce-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50bce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50bce-107">Atualiza as propriedades de um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="50bce-107">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50bce-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50bce-108">Prerequisites</span></span>
<span data-ttu-id="50bce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50bce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50bce-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50bce-111">Permission type</span></span>|<span data-ttu-id="50bce-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50bce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50bce-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50bce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50bce-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50bce-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="50bce-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50bce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50bce-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50bce-116">Not supported.</span></span>|
|<span data-ttu-id="50bce-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50bce-117">Application</span></span>|<span data-ttu-id="50bce-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50bce-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50bce-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50bce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="50bce-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50bce-120">Request headers</span></span>
|<span data-ttu-id="50bce-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50bce-121">Header</span></span>|<span data-ttu-id="50bce-122">Valor</span><span class="sxs-lookup"><span data-stu-id="50bce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50bce-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="50bce-123">Authorization</span></span>|<span data-ttu-id="50bce-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50bce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50bce-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50bce-125">Accept</span></span>|<span data-ttu-id="50bce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50bce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50bce-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50bce-127">Request body</span></span>
<span data-ttu-id="50bce-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="50bce-128">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="50bce-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="50bce-129">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="50bce-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50bce-130">Property</span></span>|<span data-ttu-id="50bce-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="50bce-131">Type</span></span>|<span data-ttu-id="50bce-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="50bce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50bce-133">id</span><span class="sxs-lookup"><span data-stu-id="50bce-133">id</span></span>|<span data-ttu-id="50bce-134">String</span><span class="sxs-lookup"><span data-stu-id="50bce-134">String</span></span>|<span data-ttu-id="50bce-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="50bce-135">Key of the entity.</span></span> <span data-ttu-id="50bce-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50bce-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50bce-137">displayName</span><span class="sxs-lookup"><span data-stu-id="50bce-137">displayName</span></span>|<span data-ttu-id="50bce-138">String</span><span class="sxs-lookup"><span data-stu-id="50bce-138">String</span></span>|<span data-ttu-id="50bce-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="50bce-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="50bce-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50bce-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50bce-141">description</span><span class="sxs-lookup"><span data-stu-id="50bce-141">description</span></span>|<span data-ttu-id="50bce-142">String</span><span class="sxs-lookup"><span data-stu-id="50bce-142">String</span></span>|<span data-ttu-id="50bce-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="50bce-143">The description of the app.</span></span> <span data-ttu-id="50bce-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50bce-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50bce-145">publicador</span><span class="sxs-lookup"><span data-stu-id="50bce-145">publisher</span></span>|<span data-ttu-id="50bce-146">String</span><span class="sxs-lookup"><span data-stu-id="50bce-146">String</span></span>|<span data-ttu-id="50bce-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="50bce-147">The publisher of the app.</span></span> <span data-ttu-id="50bce-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50bce-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50bce-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="50bce-149">largeIcon</span></span>|[<span data-ttu-id="50bce-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="50bce-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="50bce-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="50bce-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="50bce-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50bce-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50bce-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50bce-153">createdDateTime</span></span>|<span data-ttu-id="50bce-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50bce-154">DateTimeOffset</span></span>|<span data-ttu-id="50bce-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="50bce-155">The date and time the app was created.</span></span> <span data-ttu-id="50bce-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50bce-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50bce-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50bce-157">lastModifiedDateTime</span></span>|<span data-ttu-id="50bce-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50bce-158">DateTimeOffset</span></span>|<span data-ttu-id="50bce-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="50bce-159">The date and time the app was last modified.</span></span> <span data-ttu-id="50bce-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50bce-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50bce-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="50bce-161">isFeatured</span></span>|<span data-ttu-id="50bce-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="50bce-162">Boolean</span></span>|<span data-ttu-id="50bce-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50bce-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50bce-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="50bce-164">privacyInformationUrl</span></span>|<span data-ttu-id="50bce-165">String</span><span class="sxs-lookup"><span data-stu-id="50bce-165">String</span></span>|<span data-ttu-id="50bce-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="50bce-166">The privacy statement Url.</span></span> <span data-ttu-id="50bce-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50bce-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50bce-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="50bce-168">informationUrl</span></span>|<span data-ttu-id="50bce-169">String</span><span class="sxs-lookup"><span data-stu-id="50bce-169">String</span></span>|<span data-ttu-id="50bce-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="50bce-170">The more information Url.</span></span> <span data-ttu-id="50bce-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50bce-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50bce-172">owner</span><span class="sxs-lookup"><span data-stu-id="50bce-172">owner</span></span>|<span data-ttu-id="50bce-173">String</span><span class="sxs-lookup"><span data-stu-id="50bce-173">String</span></span>|<span data-ttu-id="50bce-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="50bce-174">The owner of the app.</span></span> <span data-ttu-id="50bce-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50bce-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50bce-176">developer</span><span class="sxs-lookup"><span data-stu-id="50bce-176">developer</span></span>|<span data-ttu-id="50bce-177">String</span><span class="sxs-lookup"><span data-stu-id="50bce-177">String</span></span>|<span data-ttu-id="50bce-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="50bce-178">The developer of the app.</span></span> <span data-ttu-id="50bce-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50bce-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50bce-180">notes</span><span class="sxs-lookup"><span data-stu-id="50bce-180">notes</span></span>|<span data-ttu-id="50bce-181">String</span><span class="sxs-lookup"><span data-stu-id="50bce-181">String</span></span>|<span data-ttu-id="50bce-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="50bce-182">Notes for the app.</span></span> <span data-ttu-id="50bce-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50bce-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50bce-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="50bce-184">uploadState</span></span>|<span data-ttu-id="50bce-185">Int32</span><span class="sxs-lookup"><span data-stu-id="50bce-185">Int32</span></span>|<span data-ttu-id="50bce-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="50bce-186">The upload state.</span></span> <span data-ttu-id="50bce-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="50bce-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="50bce-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50bce-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50bce-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="50bce-189">publishingState</span></span>|[<span data-ttu-id="50bce-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="50bce-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="50bce-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="50bce-191">The publishing state for the app.</span></span> <span data-ttu-id="50bce-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="50bce-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="50bce-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="50bce-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="50bce-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="50bce-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="50bce-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="50bce-195">isAssigned</span></span>|<span data-ttu-id="50bce-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="50bce-196">Boolean</span></span>|<span data-ttu-id="50bce-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="50bce-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="50bce-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50bce-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50bce-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="50bce-199">roleScopeTagIds</span></span>|<span data-ttu-id="50bce-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="50bce-200">String collection</span></span>|<span data-ttu-id="50bce-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="50bce-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="50bce-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50bce-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50bce-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="50bce-203">dependentAppCount</span></span>|<span data-ttu-id="50bce-204">Int32</span><span class="sxs-lookup"><span data-stu-id="50bce-204">Int32</span></span>|<span data-ttu-id="50bce-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="50bce-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="50bce-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50bce-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50bce-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="50bce-207">supersedingAppCount</span></span>|<span data-ttu-id="50bce-208">Int32</span><span class="sxs-lookup"><span data-stu-id="50bce-208">Int32</span></span>|<span data-ttu-id="50bce-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="50bce-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="50bce-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50bce-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50bce-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="50bce-211">supersededAppCount</span></span>|<span data-ttu-id="50bce-212">Int32</span><span class="sxs-lookup"><span data-stu-id="50bce-212">Int32</span></span>|<span data-ttu-id="50bce-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="50bce-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="50bce-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50bce-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50bce-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="50bce-215">appAvailability</span></span>|[<span data-ttu-id="50bce-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="50bce-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="50bce-217">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="50bce-217">The Application's availability.</span></span> <span data-ttu-id="50bce-218">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="50bce-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="50bce-219">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="50bce-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="50bce-220">version</span><span class="sxs-lookup"><span data-stu-id="50bce-220">version</span></span>|<span data-ttu-id="50bce-221">String</span><span class="sxs-lookup"><span data-stu-id="50bce-221">String</span></span>|<span data-ttu-id="50bce-222">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="50bce-222">The Application's version.</span></span> <span data-ttu-id="50bce-223">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="50bce-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="50bce-224">bundleId</span><span class="sxs-lookup"><span data-stu-id="50bce-224">bundleId</span></span>|<span data-ttu-id="50bce-225">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50bce-225">String</span></span>|<span data-ttu-id="50bce-226">A ID do pacote de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="50bce-226">The app's Bundle ID.</span></span>|
|<span data-ttu-id="50bce-227">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="50bce-227">appStoreUrl</span></span>|<span data-ttu-id="50bce-228">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50bce-228">String</span></span>|<span data-ttu-id="50bce-229">A AppStoreUrl da Apple.</span><span class="sxs-lookup"><span data-stu-id="50bce-229">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="50bce-230">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="50bce-230">applicableDeviceType</span></span>|[<span data-ttu-id="50bce-231">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="50bce-231">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="50bce-232">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="50bce-232">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="50bce-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="50bce-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="50bce-234">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="50bce-234">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="50bce-235">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="50bce-235">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="50bce-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="50bce-236">Response</span></span>
<span data-ttu-id="50bce-237">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50bce-237">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50bce-238">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50bce-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="50bce-239">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50bce-239">Request</span></span>
<span data-ttu-id="50bce-240">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50bce-240">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1295

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
    "v13_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="50bce-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="50bce-241">Response</span></span>
<span data-ttu-id="50bce-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50bce-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1467

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
    "v13_0": true
  }
}
```




