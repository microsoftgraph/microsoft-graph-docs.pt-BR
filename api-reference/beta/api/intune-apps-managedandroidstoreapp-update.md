---
title: Atualizar managedAndroidStoreApp
description: Atualiza as propriedades de um objeto managedAndroidStoreApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 07cd1d7ca6bbec237a853e8670437e07a06cb2a9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421043"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="43d20-103">Atualizar managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="43d20-103">Update managedAndroidStoreApp</span></span>

> <span data-ttu-id="43d20-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="43d20-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="43d20-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="43d20-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43d20-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="43d20-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43d20-107">Atualiza as propriedades de um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="43d20-107">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43d20-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="43d20-108">Prerequisites</span></span>
<span data-ttu-id="43d20-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="43d20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="43d20-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43d20-111">Permission type</span></span>|<span data-ttu-id="43d20-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="43d20-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43d20-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43d20-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43d20-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43d20-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="43d20-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43d20-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43d20-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43d20-116">Not supported.</span></span>|
|<span data-ttu-id="43d20-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43d20-117">Application</span></span>|<span data-ttu-id="43d20-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43d20-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43d20-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43d20-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="43d20-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43d20-120">Request headers</span></span>
|<span data-ttu-id="43d20-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="43d20-121">Header</span></span>|<span data-ttu-id="43d20-122">Valor</span><span class="sxs-lookup"><span data-stu-id="43d20-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43d20-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="43d20-123">Authorization</span></span>|<span data-ttu-id="43d20-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43d20-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43d20-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="43d20-125">Accept</span></span>|<span data-ttu-id="43d20-126">application/json</span><span class="sxs-lookup"><span data-stu-id="43d20-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43d20-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43d20-127">Request body</span></span>
<span data-ttu-id="43d20-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="43d20-128">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="43d20-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="43d20-129">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="43d20-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43d20-130">Property</span></span>|<span data-ttu-id="43d20-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="43d20-131">Type</span></span>|<span data-ttu-id="43d20-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="43d20-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43d20-133">id</span><span class="sxs-lookup"><span data-stu-id="43d20-133">id</span></span>|<span data-ttu-id="43d20-134">String</span><span class="sxs-lookup"><span data-stu-id="43d20-134">String</span></span>|<span data-ttu-id="43d20-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="43d20-135">Key of the entity.</span></span> <span data-ttu-id="43d20-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="43d20-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43d20-137">displayName</span><span class="sxs-lookup"><span data-stu-id="43d20-137">displayName</span></span>|<span data-ttu-id="43d20-138">String</span><span class="sxs-lookup"><span data-stu-id="43d20-138">String</span></span>|<span data-ttu-id="43d20-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="43d20-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="43d20-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="43d20-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43d20-141">description</span><span class="sxs-lookup"><span data-stu-id="43d20-141">description</span></span>|<span data-ttu-id="43d20-142">String</span><span class="sxs-lookup"><span data-stu-id="43d20-142">String</span></span>|<span data-ttu-id="43d20-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="43d20-143">The description of the app.</span></span> <span data-ttu-id="43d20-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="43d20-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43d20-145">publisher</span><span class="sxs-lookup"><span data-stu-id="43d20-145">publisher</span></span>|<span data-ttu-id="43d20-146">String</span><span class="sxs-lookup"><span data-stu-id="43d20-146">String</span></span>|<span data-ttu-id="43d20-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="43d20-147">The publisher of the app.</span></span> <span data-ttu-id="43d20-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="43d20-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43d20-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="43d20-149">largeIcon</span></span>|[<span data-ttu-id="43d20-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="43d20-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="43d20-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="43d20-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="43d20-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="43d20-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43d20-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43d20-153">createdDateTime</span></span>|<span data-ttu-id="43d20-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43d20-154">DateTimeOffset</span></span>|<span data-ttu-id="43d20-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="43d20-155">The date and time the app was created.</span></span> <span data-ttu-id="43d20-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="43d20-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43d20-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43d20-157">lastModifiedDateTime</span></span>|<span data-ttu-id="43d20-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43d20-158">DateTimeOffset</span></span>|<span data-ttu-id="43d20-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="43d20-159">The date and time the app was last modified.</span></span> <span data-ttu-id="43d20-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="43d20-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43d20-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="43d20-161">isFeatured</span></span>|<span data-ttu-id="43d20-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="43d20-162">Boolean</span></span>|<span data-ttu-id="43d20-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="43d20-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43d20-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="43d20-164">privacyInformationUrl</span></span>|<span data-ttu-id="43d20-165">String</span><span class="sxs-lookup"><span data-stu-id="43d20-165">String</span></span>|<span data-ttu-id="43d20-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="43d20-166">The privacy statement Url.</span></span> <span data-ttu-id="43d20-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="43d20-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43d20-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="43d20-168">informationUrl</span></span>|<span data-ttu-id="43d20-169">String</span><span class="sxs-lookup"><span data-stu-id="43d20-169">String</span></span>|<span data-ttu-id="43d20-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="43d20-170">The more information Url.</span></span> <span data-ttu-id="43d20-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="43d20-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43d20-172">owner</span><span class="sxs-lookup"><span data-stu-id="43d20-172">owner</span></span>|<span data-ttu-id="43d20-173">String</span><span class="sxs-lookup"><span data-stu-id="43d20-173">String</span></span>|<span data-ttu-id="43d20-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="43d20-174">The owner of the app.</span></span> <span data-ttu-id="43d20-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="43d20-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43d20-176">developer</span><span class="sxs-lookup"><span data-stu-id="43d20-176">developer</span></span>|<span data-ttu-id="43d20-177">String</span><span class="sxs-lookup"><span data-stu-id="43d20-177">String</span></span>|<span data-ttu-id="43d20-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="43d20-178">The developer of the app.</span></span> <span data-ttu-id="43d20-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="43d20-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43d20-180">Observações</span><span class="sxs-lookup"><span data-stu-id="43d20-180">notes</span></span>|<span data-ttu-id="43d20-181">String</span><span class="sxs-lookup"><span data-stu-id="43d20-181">String</span></span>|<span data-ttu-id="43d20-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="43d20-182">Notes for the app.</span></span> <span data-ttu-id="43d20-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="43d20-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43d20-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="43d20-184">uploadState</span></span>|<span data-ttu-id="43d20-185">Int32</span><span class="sxs-lookup"><span data-stu-id="43d20-185">Int32</span></span>|<span data-ttu-id="43d20-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="43d20-186">The upload state.</span></span> <span data-ttu-id="43d20-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="43d20-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43d20-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="43d20-188">publishingState</span></span>|[<span data-ttu-id="43d20-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="43d20-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="43d20-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="43d20-190">The publishing state for the app.</span></span> <span data-ttu-id="43d20-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="43d20-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="43d20-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="43d20-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="43d20-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="43d20-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="43d20-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="43d20-194">isAssigned</span></span>|<span data-ttu-id="43d20-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="43d20-195">Boolean</span></span>|<span data-ttu-id="43d20-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="43d20-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="43d20-197">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="43d20-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43d20-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="43d20-198">roleScopeTagIds</span></span>|<span data-ttu-id="43d20-199">String collection</span><span class="sxs-lookup"><span data-stu-id="43d20-199">String collection</span></span>|<span data-ttu-id="43d20-200">Lista de ids de marca de escopo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="43d20-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="43d20-201">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="43d20-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="43d20-202">appAvailability</span><span class="sxs-lookup"><span data-stu-id="43d20-202">appAvailability</span></span>|[<span data-ttu-id="43d20-203">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="43d20-203">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="43d20-204">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="43d20-204">The Application's availability.</span></span> <span data-ttu-id="43d20-205">Herdada do [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="43d20-205">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="43d20-206">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="43d20-206">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="43d20-207">version</span><span class="sxs-lookup"><span data-stu-id="43d20-207">version</span></span>|<span data-ttu-id="43d20-208">String</span><span class="sxs-lookup"><span data-stu-id="43d20-208">String</span></span>|<span data-ttu-id="43d20-209">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="43d20-209">The Application's version.</span></span> <span data-ttu-id="43d20-210">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="43d20-210">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="43d20-211">packageId</span><span class="sxs-lookup"><span data-stu-id="43d20-211">packageId</span></span>|<span data-ttu-id="43d20-212">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43d20-212">String</span></span>|<span data-ttu-id="43d20-213">A ID de pacote do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="43d20-213">The app's package ID.</span></span>|
|<span data-ttu-id="43d20-214">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="43d20-214">appStoreUrl</span></span>|<span data-ttu-id="43d20-215">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43d20-215">String</span></span>|<span data-ttu-id="43d20-216">A AppStoreUrl do Android.</span><span class="sxs-lookup"><span data-stu-id="43d20-216">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="43d20-217">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="43d20-217">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="43d20-218">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="43d20-218">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="43d20-219">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="43d20-219">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="43d20-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="43d20-220">Response</span></span>
<span data-ttu-id="43d20-221">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43d20-221">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43d20-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43d20-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="43d20-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43d20-223">Request</span></span>
<span data-ttu-id="43d20-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="43d20-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="43d20-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="43d20-225">Response</span></span>
<span data-ttu-id="43d20-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43d20-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




