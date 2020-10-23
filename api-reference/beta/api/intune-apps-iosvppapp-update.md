---
title: Atualizar iosVppApp
description: Atualiza as propriedades de um objeto iosVppApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b8c46aa15bd5d69ef709194f38810da51f15ab8a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700147"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="ca95d-103">Atualizar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="ca95d-103">Update iosVppApp</span></span>

<span data-ttu-id="ca95d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca95d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca95d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ca95d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca95d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ca95d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca95d-107">Atualiza as propriedades de um objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="ca95d-107">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca95d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ca95d-108">Prerequisites</span></span>
<span data-ttu-id="ca95d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca95d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca95d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca95d-111">Permission type</span></span>|<span data-ttu-id="ca95d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ca95d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca95d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca95d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca95d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca95d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ca95d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca95d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca95d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca95d-116">Not supported.</span></span>|
|<span data-ttu-id="ca95d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca95d-117">Application</span></span>|<span data-ttu-id="ca95d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca95d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca95d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca95d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="ca95d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca95d-120">Request headers</span></span>
|<span data-ttu-id="ca95d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca95d-121">Header</span></span>|<span data-ttu-id="ca95d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ca95d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca95d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca95d-123">Authorization</span></span>|<span data-ttu-id="ca95d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca95d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca95d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ca95d-125">Accept</span></span>|<span data-ttu-id="ca95d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca95d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca95d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca95d-127">Request body</span></span>
<span data-ttu-id="ca95d-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="ca95d-128">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="ca95d-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="ca95d-129">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="ca95d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca95d-130">Property</span></span>|<span data-ttu-id="ca95d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca95d-131">Type</span></span>|<span data-ttu-id="ca95d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca95d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca95d-133">id</span><span class="sxs-lookup"><span data-stu-id="ca95d-133">id</span></span>|<span data-ttu-id="ca95d-134">String</span><span class="sxs-lookup"><span data-stu-id="ca95d-134">String</span></span>|<span data-ttu-id="ca95d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ca95d-135">Key of the entity.</span></span> <span data-ttu-id="ca95d-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca95d-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ca95d-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ca95d-137">displayName</span></span>|<span data-ttu-id="ca95d-138">String</span><span class="sxs-lookup"><span data-stu-id="ca95d-138">String</span></span>|<span data-ttu-id="ca95d-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ca95d-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ca95d-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca95d-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ca95d-141">description</span><span class="sxs-lookup"><span data-stu-id="ca95d-141">description</span></span>|<span data-ttu-id="ca95d-142">String</span><span class="sxs-lookup"><span data-stu-id="ca95d-142">String</span></span>|<span data-ttu-id="ca95d-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ca95d-143">The description of the app.</span></span> <span data-ttu-id="ca95d-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca95d-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ca95d-145">publicador</span><span class="sxs-lookup"><span data-stu-id="ca95d-145">publisher</span></span>|<span data-ttu-id="ca95d-146">String</span><span class="sxs-lookup"><span data-stu-id="ca95d-146">String</span></span>|<span data-ttu-id="ca95d-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ca95d-147">The publisher of the app.</span></span> <span data-ttu-id="ca95d-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca95d-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ca95d-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ca95d-149">largeIcon</span></span>|[<span data-ttu-id="ca95d-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ca95d-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ca95d-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="ca95d-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ca95d-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca95d-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ca95d-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ca95d-153">createdDateTime</span></span>|<span data-ttu-id="ca95d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca95d-154">DateTimeOffset</span></span>|<span data-ttu-id="ca95d-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ca95d-155">The date and time the app was created.</span></span> <span data-ttu-id="ca95d-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca95d-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ca95d-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca95d-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ca95d-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca95d-158">DateTimeOffset</span></span>|<span data-ttu-id="ca95d-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ca95d-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ca95d-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca95d-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ca95d-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ca95d-161">isFeatured</span></span>|<span data-ttu-id="ca95d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca95d-162">Boolean</span></span>|<span data-ttu-id="ca95d-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca95d-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ca95d-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ca95d-164">privacyInformationUrl</span></span>|<span data-ttu-id="ca95d-165">String</span><span class="sxs-lookup"><span data-stu-id="ca95d-165">String</span></span>|<span data-ttu-id="ca95d-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="ca95d-166">The privacy statement Url.</span></span> <span data-ttu-id="ca95d-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca95d-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ca95d-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ca95d-168">informationUrl</span></span>|<span data-ttu-id="ca95d-169">String</span><span class="sxs-lookup"><span data-stu-id="ca95d-169">String</span></span>|<span data-ttu-id="ca95d-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="ca95d-170">The more information Url.</span></span> <span data-ttu-id="ca95d-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca95d-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ca95d-172">owner</span><span class="sxs-lookup"><span data-stu-id="ca95d-172">owner</span></span>|<span data-ttu-id="ca95d-173">String</span><span class="sxs-lookup"><span data-stu-id="ca95d-173">String</span></span>|<span data-ttu-id="ca95d-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ca95d-174">The owner of the app.</span></span> <span data-ttu-id="ca95d-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca95d-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ca95d-176">developer</span><span class="sxs-lookup"><span data-stu-id="ca95d-176">developer</span></span>|<span data-ttu-id="ca95d-177">String</span><span class="sxs-lookup"><span data-stu-id="ca95d-177">String</span></span>|<span data-ttu-id="ca95d-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ca95d-178">The developer of the app.</span></span> <span data-ttu-id="ca95d-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca95d-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ca95d-180">notes</span><span class="sxs-lookup"><span data-stu-id="ca95d-180">notes</span></span>|<span data-ttu-id="ca95d-181">String</span><span class="sxs-lookup"><span data-stu-id="ca95d-181">String</span></span>|<span data-ttu-id="ca95d-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ca95d-182">Notes for the app.</span></span> <span data-ttu-id="ca95d-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca95d-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ca95d-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ca95d-184">uploadState</span></span>|<span data-ttu-id="ca95d-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ca95d-185">Int32</span></span>|<span data-ttu-id="ca95d-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="ca95d-186">The upload state.</span></span> <span data-ttu-id="ca95d-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="ca95d-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="ca95d-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca95d-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ca95d-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="ca95d-189">publishingState</span></span>|[<span data-ttu-id="ca95d-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ca95d-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ca95d-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ca95d-191">The publishing state for the app.</span></span> <span data-ttu-id="ca95d-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="ca95d-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ca95d-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ca95d-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="ca95d-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ca95d-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ca95d-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ca95d-195">isAssigned</span></span>|<span data-ttu-id="ca95d-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca95d-196">Boolean</span></span>|<span data-ttu-id="ca95d-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="ca95d-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ca95d-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca95d-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ca95d-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ca95d-199">roleScopeTagIds</span></span>|<span data-ttu-id="ca95d-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca95d-200">String collection</span></span>|<span data-ttu-id="ca95d-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="ca95d-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ca95d-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca95d-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ca95d-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="ca95d-203">dependentAppCount</span></span>|<span data-ttu-id="ca95d-204">Int32</span><span class="sxs-lookup"><span data-stu-id="ca95d-204">Int32</span></span>|<span data-ttu-id="ca95d-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="ca95d-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="ca95d-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca95d-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ca95d-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="ca95d-207">supersedingAppCount</span></span>|<span data-ttu-id="ca95d-208">Int32</span><span class="sxs-lookup"><span data-stu-id="ca95d-208">Int32</span></span>|<span data-ttu-id="ca95d-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="ca95d-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="ca95d-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca95d-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ca95d-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="ca95d-211">supersededAppCount</span></span>|<span data-ttu-id="ca95d-212">Int32</span><span class="sxs-lookup"><span data-stu-id="ca95d-212">Int32</span></span>|<span data-ttu-id="ca95d-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="ca95d-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="ca95d-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ca95d-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ca95d-215">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="ca95d-215">usedLicenseCount</span></span>|<span data-ttu-id="ca95d-216">Int32</span><span class="sxs-lookup"><span data-stu-id="ca95d-216">Int32</span></span>|<span data-ttu-id="ca95d-217">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="ca95d-217">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="ca95d-218">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="ca95d-218">totalLicenseCount</span></span>|<span data-ttu-id="ca95d-219">Int32</span><span class="sxs-lookup"><span data-stu-id="ca95d-219">Int32</span></span>|<span data-ttu-id="ca95d-220">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="ca95d-220">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="ca95d-221">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="ca95d-221">releaseDateTime</span></span>|<span data-ttu-id="ca95d-222">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca95d-222">DateTimeOffset</span></span>|<span data-ttu-id="ca95d-223">A data e a hora de lançamento do aplicativo VPP.</span><span class="sxs-lookup"><span data-stu-id="ca95d-223">The VPP application release date and time.</span></span>|
|<span data-ttu-id="ca95d-224">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ca95d-224">appStoreUrl</span></span>|<span data-ttu-id="ca95d-225">String</span><span class="sxs-lookup"><span data-stu-id="ca95d-225">String</span></span>|<span data-ttu-id="ca95d-226">A URL da loja.</span><span class="sxs-lookup"><span data-stu-id="ca95d-226">The store URL.</span></span>|
|<span data-ttu-id="ca95d-227">licensingType</span><span class="sxs-lookup"><span data-stu-id="ca95d-227">licensingType</span></span>|[<span data-ttu-id="ca95d-228">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="ca95d-228">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="ca95d-229">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="ca95d-229">The supported License Type.</span></span>|
|<span data-ttu-id="ca95d-230">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="ca95d-230">applicableDeviceType</span></span>|[<span data-ttu-id="ca95d-231">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="ca95d-231">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="ca95d-232">O tipo de dispositivo iOS aplicável.</span><span class="sxs-lookup"><span data-stu-id="ca95d-232">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="ca95d-233">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="ca95d-233">vppTokenOrganizationName</span></span>|<span data-ttu-id="ca95d-234">String</span><span class="sxs-lookup"><span data-stu-id="ca95d-234">String</span></span>|<span data-ttu-id="ca95d-235">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="ca95d-235">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="ca95d-236">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="ca95d-236">vppTokenAccountType</span></span>|[<span data-ttu-id="ca95d-237">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="ca95d-237">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="ca95d-238">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="ca95d-238">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="ca95d-239">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="ca95d-239">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="ca95d-240">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="ca95d-240">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="ca95d-241">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="ca95d-241">vppTokenAppleId</span></span>|<span data-ttu-id="ca95d-242">String</span><span class="sxs-lookup"><span data-stu-id="ca95d-242">String</span></span>|<span data-ttu-id="ca95d-243">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="ca95d-243">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ca95d-244">bundleId</span><span class="sxs-lookup"><span data-stu-id="ca95d-244">bundleId</span></span>|<span data-ttu-id="ca95d-245">String</span><span class="sxs-lookup"><span data-stu-id="ca95d-245">String</span></span>|<span data-ttu-id="ca95d-246">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="ca95d-246">The Identity Name.</span></span>|
|<span data-ttu-id="ca95d-247">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="ca95d-247">vppTokenId</span></span>|<span data-ttu-id="ca95d-248">String</span><span class="sxs-lookup"><span data-stu-id="ca95d-248">String</span></span>|<span data-ttu-id="ca95d-249">Identificador do token VPP associado a este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ca95d-249">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="ca95d-250">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="ca95d-250">revokeLicenseActionResults</span></span>|<span data-ttu-id="ca95d-251">coleção [iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ca95d-251">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="ca95d-252">Resultados da revogação de ações de licença neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ca95d-252">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="ca95d-253">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca95d-253">Response</span></span>
<span data-ttu-id="ca95d-254">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [iosVppApp](../resources/intune-apps-iosvppapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca95d-254">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca95d-255">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca95d-255">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca95d-256">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca95d-256">Request</span></span>
<span data-ttu-id="ca95d-257">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca95d-257">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2056

{
  "@odata.type": "#microsoft.graph.iosVppApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="ca95d-258">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca95d-258">Response</span></span>
<span data-ttu-id="ca95d-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca95d-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2228

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```





