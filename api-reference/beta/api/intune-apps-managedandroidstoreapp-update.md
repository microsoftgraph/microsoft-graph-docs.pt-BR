---
title: Atualizar managedAndroidStoreApp
description: Atualiza as propriedades de um objeto managedAndroidStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0134cc874ee50a9b3a46b24b9d3a1154499b7bd2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173910"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="54427-103">Atualizar managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="54427-103">Update managedAndroidStoreApp</span></span>

> <span data-ttu-id="54427-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="54427-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54427-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="54427-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54427-106">Atualiza as propriedades de um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="54427-106">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54427-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="54427-107">Prerequisites</span></span>
<span data-ttu-id="54427-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="54427-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="54427-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54427-110">Permission type</span></span>|<span data-ttu-id="54427-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="54427-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54427-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54427-112">Delegated (work or school account)</span></span>|<span data-ttu-id="54427-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54427-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="54427-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54427-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54427-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54427-115">Not supported.</span></span>|
|<span data-ttu-id="54427-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54427-116">Application</span></span>|<span data-ttu-id="54427-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54427-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54427-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54427-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="54427-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54427-119">Request headers</span></span>
|<span data-ttu-id="54427-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="54427-120">Header</span></span>|<span data-ttu-id="54427-121">Valor</span><span class="sxs-lookup"><span data-stu-id="54427-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54427-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="54427-122">Authorization</span></span>|<span data-ttu-id="54427-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54427-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54427-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="54427-124">Accept</span></span>|<span data-ttu-id="54427-125">application/json</span><span class="sxs-lookup"><span data-stu-id="54427-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54427-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54427-126">Request body</span></span>
<span data-ttu-id="54427-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="54427-127">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="54427-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="54427-128">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="54427-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54427-129">Property</span></span>|<span data-ttu-id="54427-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="54427-130">Type</span></span>|<span data-ttu-id="54427-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="54427-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54427-132">id</span><span class="sxs-lookup"><span data-stu-id="54427-132">id</span></span>|<span data-ttu-id="54427-133">String</span><span class="sxs-lookup"><span data-stu-id="54427-133">String</span></span>|<span data-ttu-id="54427-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="54427-134">Key of the entity.</span></span> <span data-ttu-id="54427-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54427-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54427-136">displayName</span><span class="sxs-lookup"><span data-stu-id="54427-136">displayName</span></span>|<span data-ttu-id="54427-137">String</span><span class="sxs-lookup"><span data-stu-id="54427-137">String</span></span>|<span data-ttu-id="54427-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="54427-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="54427-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54427-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54427-140">description</span><span class="sxs-lookup"><span data-stu-id="54427-140">description</span></span>|<span data-ttu-id="54427-141">String</span><span class="sxs-lookup"><span data-stu-id="54427-141">String</span></span>|<span data-ttu-id="54427-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="54427-142">The description of the app.</span></span> <span data-ttu-id="54427-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54427-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54427-144">publisher</span><span class="sxs-lookup"><span data-stu-id="54427-144">publisher</span></span>|<span data-ttu-id="54427-145">String</span><span class="sxs-lookup"><span data-stu-id="54427-145">String</span></span>|<span data-ttu-id="54427-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="54427-146">The publisher of the app.</span></span> <span data-ttu-id="54427-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54427-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54427-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="54427-148">largeIcon</span></span>|[<span data-ttu-id="54427-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="54427-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="54427-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="54427-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="54427-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54427-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54427-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54427-152">createdDateTime</span></span>|<span data-ttu-id="54427-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54427-153">DateTimeOffset</span></span>|<span data-ttu-id="54427-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="54427-154">The date and time the app was created.</span></span> <span data-ttu-id="54427-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54427-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54427-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54427-156">lastModifiedDateTime</span></span>|<span data-ttu-id="54427-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54427-157">DateTimeOffset</span></span>|<span data-ttu-id="54427-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="54427-158">The date and time the app was last modified.</span></span> <span data-ttu-id="54427-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54427-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54427-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="54427-160">isFeatured</span></span>|<span data-ttu-id="54427-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="54427-161">Boolean</span></span>|<span data-ttu-id="54427-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54427-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54427-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="54427-163">privacyInformationUrl</span></span>|<span data-ttu-id="54427-164">String</span><span class="sxs-lookup"><span data-stu-id="54427-164">String</span></span>|<span data-ttu-id="54427-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="54427-165">The privacy statement Url.</span></span> <span data-ttu-id="54427-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54427-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54427-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="54427-167">informationUrl</span></span>|<span data-ttu-id="54427-168">String</span><span class="sxs-lookup"><span data-stu-id="54427-168">String</span></span>|<span data-ttu-id="54427-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="54427-169">The more information Url.</span></span> <span data-ttu-id="54427-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54427-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54427-171">owner</span><span class="sxs-lookup"><span data-stu-id="54427-171">owner</span></span>|<span data-ttu-id="54427-172">String</span><span class="sxs-lookup"><span data-stu-id="54427-172">String</span></span>|<span data-ttu-id="54427-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="54427-173">The owner of the app.</span></span> <span data-ttu-id="54427-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54427-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54427-175">developer</span><span class="sxs-lookup"><span data-stu-id="54427-175">developer</span></span>|<span data-ttu-id="54427-176">String</span><span class="sxs-lookup"><span data-stu-id="54427-176">String</span></span>|<span data-ttu-id="54427-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="54427-177">The developer of the app.</span></span> <span data-ttu-id="54427-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54427-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54427-179">Observações</span><span class="sxs-lookup"><span data-stu-id="54427-179">notes</span></span>|<span data-ttu-id="54427-180">String</span><span class="sxs-lookup"><span data-stu-id="54427-180">String</span></span>|<span data-ttu-id="54427-181">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="54427-181">Notes for the app.</span></span> <span data-ttu-id="54427-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54427-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54427-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="54427-183">uploadState</span></span>|<span data-ttu-id="54427-184">Int32</span><span class="sxs-lookup"><span data-stu-id="54427-184">Int32</span></span>|<span data-ttu-id="54427-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="54427-185">The upload state.</span></span> <span data-ttu-id="54427-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54427-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54427-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="54427-187">publishingState</span></span>|[<span data-ttu-id="54427-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="54427-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="54427-189">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="54427-189">The publishing state for the app.</span></span> <span data-ttu-id="54427-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="54427-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="54427-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="54427-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="54427-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="54427-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="54427-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="54427-193">isAssigned</span></span>|<span data-ttu-id="54427-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="54427-194">Boolean</span></span>|<span data-ttu-id="54427-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="54427-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="54427-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54427-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54427-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="54427-197">roleScopeTagIds</span></span>|<span data-ttu-id="54427-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="54427-198">String collection</span></span>|<span data-ttu-id="54427-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="54427-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="54427-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="54427-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="54427-201">appAvailability</span><span class="sxs-lookup"><span data-stu-id="54427-201">appAvailability</span></span>|[<span data-ttu-id="54427-202">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="54427-202">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="54427-203">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="54427-203">The Application's availability.</span></span> <span data-ttu-id="54427-204">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="54427-204">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="54427-205">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="54427-205">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="54427-206">version</span><span class="sxs-lookup"><span data-stu-id="54427-206">version</span></span>|<span data-ttu-id="54427-207">String</span><span class="sxs-lookup"><span data-stu-id="54427-207">String</span></span>|<span data-ttu-id="54427-208">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="54427-208">The Application's version.</span></span> <span data-ttu-id="54427-209">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="54427-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="54427-210">packageId</span><span class="sxs-lookup"><span data-stu-id="54427-210">packageId</span></span>|<span data-ttu-id="54427-211">String</span><span class="sxs-lookup"><span data-stu-id="54427-211">String</span></span>|<span data-ttu-id="54427-212">A ID de pacote do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="54427-212">The app's package ID.</span></span>|
|<span data-ttu-id="54427-213">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="54427-213">appStoreUrl</span></span>|<span data-ttu-id="54427-214">String</span><span class="sxs-lookup"><span data-stu-id="54427-214">String</span></span>|<span data-ttu-id="54427-215">A AppStoreUrl do Android.</span><span class="sxs-lookup"><span data-stu-id="54427-215">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="54427-216">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="54427-216">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="54427-217">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="54427-217">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="54427-218">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="54427-218">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="54427-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="54427-219">Response</span></span>
<span data-ttu-id="54427-220">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54427-220">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54427-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54427-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="54427-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54427-222">Request</span></span>
<span data-ttu-id="54427-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54427-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1237

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
    "v9_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="54427-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="54427-224">Response</span></span>
<span data-ttu-id="54427-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54427-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1409

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
    "v9_0": true
  }
}
```




