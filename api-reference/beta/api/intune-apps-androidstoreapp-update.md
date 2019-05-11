---
title: Atualizar androidStoreApp
description: Atualiza as propriedades de um objeto androidStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 580fc24bbc82a585430250d1b0e2125a01f106b6
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33937257"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="39e1e-103">Atualizar androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="39e1e-103">Update androidStoreApp</span></span>

> <span data-ttu-id="39e1e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="39e1e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39e1e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="39e1e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39e1e-106">Atualiza as propriedades de um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="39e1e-106">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39e1e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="39e1e-107">Prerequisites</span></span>
<span data-ttu-id="39e1e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39e1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39e1e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39e1e-110">Permission type</span></span>|<span data-ttu-id="39e1e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="39e1e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39e1e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39e1e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="39e1e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39e1e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="39e1e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39e1e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39e1e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39e1e-115">Not supported.</span></span>|
|<span data-ttu-id="39e1e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39e1e-116">Application</span></span>|<span data-ttu-id="39e1e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39e1e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39e1e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39e1e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="39e1e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39e1e-119">Request headers</span></span>
|<span data-ttu-id="39e1e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="39e1e-120">Header</span></span>|<span data-ttu-id="39e1e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="39e1e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39e1e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="39e1e-122">Authorization</span></span>|<span data-ttu-id="39e1e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39e1e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39e1e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="39e1e-124">Accept</span></span>|<span data-ttu-id="39e1e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="39e1e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39e1e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39e1e-126">Request body</span></span>
<span data-ttu-id="39e1e-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="39e1e-127">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="39e1e-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="39e1e-128">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="39e1e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39e1e-129">Property</span></span>|<span data-ttu-id="39e1e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="39e1e-130">Type</span></span>|<span data-ttu-id="39e1e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="39e1e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39e1e-132">id</span><span class="sxs-lookup"><span data-stu-id="39e1e-132">id</span></span>|<span data-ttu-id="39e1e-133">String</span><span class="sxs-lookup"><span data-stu-id="39e1e-133">String</span></span>|<span data-ttu-id="39e1e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="39e1e-134">Key of the entity.</span></span> <span data-ttu-id="39e1e-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39e1e-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39e1e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="39e1e-136">displayName</span></span>|<span data-ttu-id="39e1e-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39e1e-137">String</span></span>|<span data-ttu-id="39e1e-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="39e1e-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="39e1e-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39e1e-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39e1e-140">description</span><span class="sxs-lookup"><span data-stu-id="39e1e-140">description</span></span>|<span data-ttu-id="39e1e-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39e1e-141">String</span></span>|<span data-ttu-id="39e1e-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="39e1e-142">The description of the app.</span></span> <span data-ttu-id="39e1e-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39e1e-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39e1e-144">publicador</span><span class="sxs-lookup"><span data-stu-id="39e1e-144">publisher</span></span>|<span data-ttu-id="39e1e-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39e1e-145">String</span></span>|<span data-ttu-id="39e1e-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="39e1e-146">The publisher of the app.</span></span> <span data-ttu-id="39e1e-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39e1e-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39e1e-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="39e1e-148">largeIcon</span></span>|[<span data-ttu-id="39e1e-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="39e1e-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="39e1e-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="39e1e-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="39e1e-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39e1e-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39e1e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39e1e-152">createdDateTime</span></span>|<span data-ttu-id="39e1e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39e1e-153">DateTimeOffset</span></span>|<span data-ttu-id="39e1e-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="39e1e-154">The date and time the app was created.</span></span> <span data-ttu-id="39e1e-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39e1e-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39e1e-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39e1e-156">lastModifiedDateTime</span></span>|<span data-ttu-id="39e1e-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39e1e-157">DateTimeOffset</span></span>|<span data-ttu-id="39e1e-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="39e1e-158">The date and time the app was last modified.</span></span> <span data-ttu-id="39e1e-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39e1e-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39e1e-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="39e1e-160">isFeatured</span></span>|<span data-ttu-id="39e1e-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="39e1e-161">Boolean</span></span>|<span data-ttu-id="39e1e-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39e1e-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39e1e-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="39e1e-163">privacyInformationUrl</span></span>|<span data-ttu-id="39e1e-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39e1e-164">String</span></span>|<span data-ttu-id="39e1e-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="39e1e-165">The privacy statement Url.</span></span> <span data-ttu-id="39e1e-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39e1e-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39e1e-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="39e1e-167">informationUrl</span></span>|<span data-ttu-id="39e1e-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39e1e-168">String</span></span>|<span data-ttu-id="39e1e-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="39e1e-169">The more information Url.</span></span> <span data-ttu-id="39e1e-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39e1e-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39e1e-171">owner</span><span class="sxs-lookup"><span data-stu-id="39e1e-171">owner</span></span>|<span data-ttu-id="39e1e-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39e1e-172">String</span></span>|<span data-ttu-id="39e1e-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="39e1e-173">The owner of the app.</span></span> <span data-ttu-id="39e1e-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39e1e-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39e1e-175">developer</span><span class="sxs-lookup"><span data-stu-id="39e1e-175">developer</span></span>|<span data-ttu-id="39e1e-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39e1e-176">String</span></span>|<span data-ttu-id="39e1e-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="39e1e-177">The developer of the app.</span></span> <span data-ttu-id="39e1e-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39e1e-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39e1e-179">notes</span><span class="sxs-lookup"><span data-stu-id="39e1e-179">notes</span></span>|<span data-ttu-id="39e1e-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39e1e-180">String</span></span>|<span data-ttu-id="39e1e-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="39e1e-181">Notes for the app.</span></span> <span data-ttu-id="39e1e-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39e1e-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39e1e-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="39e1e-183">uploadState</span></span>|<span data-ttu-id="39e1e-184">Int32</span><span class="sxs-lookup"><span data-stu-id="39e1e-184">Int32</span></span>|<span data-ttu-id="39e1e-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="39e1e-185">The upload state.</span></span> <span data-ttu-id="39e1e-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39e1e-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39e1e-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="39e1e-187">publishingState</span></span>|[<span data-ttu-id="39e1e-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="39e1e-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="39e1e-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="39e1e-189">The publishing state for the app.</span></span> <span data-ttu-id="39e1e-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="39e1e-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="39e1e-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="39e1e-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="39e1e-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="39e1e-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="39e1e-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="39e1e-193">isAssigned</span></span>|<span data-ttu-id="39e1e-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="39e1e-194">Boolean</span></span>|<span data-ttu-id="39e1e-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="39e1e-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="39e1e-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39e1e-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39e1e-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="39e1e-197">roleScopeTagIds</span></span>|<span data-ttu-id="39e1e-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="39e1e-198">String collection</span></span>|<span data-ttu-id="39e1e-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="39e1e-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="39e1e-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39e1e-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39e1e-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="39e1e-201">dependentAppCount</span></span>|<span data-ttu-id="39e1e-202">Int32</span><span class="sxs-lookup"><span data-stu-id="39e1e-202">Int32</span></span>|<span data-ttu-id="39e1e-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="39e1e-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="39e1e-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39e1e-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39e1e-205">packageId</span><span class="sxs-lookup"><span data-stu-id="39e1e-205">packageId</span></span>|<span data-ttu-id="39e1e-206">String</span><span class="sxs-lookup"><span data-stu-id="39e1e-206">String</span></span>|<span data-ttu-id="39e1e-207">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="39e1e-207">The package identifier.</span></span>|
|<span data-ttu-id="39e1e-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="39e1e-208">appIdentifier</span></span>|<span data-ttu-id="39e1e-209">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39e1e-209">String</span></span>|<span data-ttu-id="39e1e-210">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="39e1e-210">The Identity Name.</span></span>|
|<span data-ttu-id="39e1e-211">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="39e1e-211">appStoreUrl</span></span>|<span data-ttu-id="39e1e-212">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39e1e-212">String</span></span>|<span data-ttu-id="39e1e-213">A URL da loja de aplicativos Android.</span><span class="sxs-lookup"><span data-stu-id="39e1e-213">The Android app store URL.</span></span>|
|<span data-ttu-id="39e1e-214">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="39e1e-214">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="39e1e-215">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="39e1e-215">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="39e1e-216">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="39e1e-216">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="39e1e-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="39e1e-217">Response</span></span>
<span data-ttu-id="39e1e-218">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39e1e-218">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39e1e-219">Exemplo</span><span class="sxs-lookup"><span data-stu-id="39e1e-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="39e1e-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39e1e-220">Request</span></span>
<span data-ttu-id="39e1e-221">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="39e1e-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1230

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
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

### <a name="response"></a><span data-ttu-id="39e1e-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="39e1e-222">Response</span></span>
<span data-ttu-id="39e1e-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="39e1e-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1402

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
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




