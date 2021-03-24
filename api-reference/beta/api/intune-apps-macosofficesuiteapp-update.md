---
title: Atualizar macOSOfficeSuiteApp
description: Atualizar as propriedades de um objeto  macOSOfficeSuiteApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c95a0c5a45a80677d24861132176b1f1949e0d74
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140396"
---
# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="45420-103">Atualizar macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="45420-103">Update macOSOfficeSuiteApp</span></span>

<span data-ttu-id="45420-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45420-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45420-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45420-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45420-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45420-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45420-107">Atualizar as propriedades de um objeto [ macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="45420-107">Update the properties of a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45420-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45420-108">Prerequisites</span></span>
<span data-ttu-id="45420-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45420-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45420-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45420-111">Permission type</span></span>|<span data-ttu-id="45420-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45420-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45420-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45420-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45420-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45420-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="45420-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45420-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45420-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45420-116">Not supported.</span></span>|
|<span data-ttu-id="45420-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45420-117">Application</span></span>|<span data-ttu-id="45420-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45420-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="45420-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45420-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="45420-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45420-120">Request headers</span></span>
|<span data-ttu-id="45420-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45420-121">Header</span></span>|<span data-ttu-id="45420-122">Valor</span><span class="sxs-lookup"><span data-stu-id="45420-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45420-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="45420-123">Authorization</span></span>|<span data-ttu-id="45420-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45420-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45420-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="45420-125">Accept</span></span>|<span data-ttu-id="45420-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45420-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45420-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45420-127">Request body</span></span>
<span data-ttu-id="45420-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="45420-128">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="45420-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="45420-129">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="45420-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45420-130">Property</span></span>|<span data-ttu-id="45420-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="45420-131">Type</span></span>|<span data-ttu-id="45420-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="45420-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45420-133">id</span><span class="sxs-lookup"><span data-stu-id="45420-133">id</span></span>|<span data-ttu-id="45420-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45420-134">String</span></span>|<span data-ttu-id="45420-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="45420-135">Key of the entity.</span></span> <span data-ttu-id="45420-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45420-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45420-137">displayName</span><span class="sxs-lookup"><span data-stu-id="45420-137">displayName</span></span>|<span data-ttu-id="45420-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45420-138">String</span></span>|<span data-ttu-id="45420-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="45420-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="45420-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45420-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45420-141">descrição</span><span class="sxs-lookup"><span data-stu-id="45420-141">description</span></span>|<span data-ttu-id="45420-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45420-142">String</span></span>|<span data-ttu-id="45420-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="45420-143">The description of the app.</span></span> <span data-ttu-id="45420-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45420-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45420-145">publicador</span><span class="sxs-lookup"><span data-stu-id="45420-145">publisher</span></span>|<span data-ttu-id="45420-146">String</span><span class="sxs-lookup"><span data-stu-id="45420-146">String</span></span>|<span data-ttu-id="45420-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="45420-147">The publisher of the app.</span></span> <span data-ttu-id="45420-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45420-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45420-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="45420-149">largeIcon</span></span>|[<span data-ttu-id="45420-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="45420-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="45420-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="45420-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="45420-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45420-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45420-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="45420-153">createdDateTime</span></span>|<span data-ttu-id="45420-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45420-154">DateTimeOffset</span></span>|<span data-ttu-id="45420-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="45420-155">The date and time the app was created.</span></span> <span data-ttu-id="45420-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45420-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45420-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45420-157">lastModifiedDateTime</span></span>|<span data-ttu-id="45420-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45420-158">DateTimeOffset</span></span>|<span data-ttu-id="45420-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="45420-159">The date and time the app was last modified.</span></span> <span data-ttu-id="45420-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45420-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45420-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="45420-161">isFeatured</span></span>|<span data-ttu-id="45420-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="45420-162">Boolean</span></span>|<span data-ttu-id="45420-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45420-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45420-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="45420-164">privacyInformationUrl</span></span>|<span data-ttu-id="45420-165">String</span><span class="sxs-lookup"><span data-stu-id="45420-165">String</span></span>|<span data-ttu-id="45420-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="45420-166">The privacy statement Url.</span></span> <span data-ttu-id="45420-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45420-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45420-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="45420-168">informationUrl</span></span>|<span data-ttu-id="45420-169">String</span><span class="sxs-lookup"><span data-stu-id="45420-169">String</span></span>|<span data-ttu-id="45420-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="45420-170">The more information Url.</span></span> <span data-ttu-id="45420-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45420-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45420-172">owner</span><span class="sxs-lookup"><span data-stu-id="45420-172">owner</span></span>|<span data-ttu-id="45420-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45420-173">String</span></span>|<span data-ttu-id="45420-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="45420-174">The owner of the app.</span></span> <span data-ttu-id="45420-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45420-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45420-176">developer</span><span class="sxs-lookup"><span data-stu-id="45420-176">developer</span></span>|<span data-ttu-id="45420-177">String</span><span class="sxs-lookup"><span data-stu-id="45420-177">String</span></span>|<span data-ttu-id="45420-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="45420-178">The developer of the app.</span></span> <span data-ttu-id="45420-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45420-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45420-180">notes</span><span class="sxs-lookup"><span data-stu-id="45420-180">notes</span></span>|<span data-ttu-id="45420-181">String</span><span class="sxs-lookup"><span data-stu-id="45420-181">String</span></span>|<span data-ttu-id="45420-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="45420-182">Notes for the app.</span></span> <span data-ttu-id="45420-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45420-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45420-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="45420-184">uploadState</span></span>|<span data-ttu-id="45420-185">Int32</span><span class="sxs-lookup"><span data-stu-id="45420-185">Int32</span></span>|<span data-ttu-id="45420-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="45420-186">The upload state.</span></span> <span data-ttu-id="45420-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="45420-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="45420-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45420-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45420-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="45420-189">publishingState</span></span>|[<span data-ttu-id="45420-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="45420-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="45420-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="45420-191">The publishing state for the app.</span></span> <span data-ttu-id="45420-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="45420-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="45420-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45420-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="45420-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="45420-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="45420-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="45420-195">isAssigned</span></span>|<span data-ttu-id="45420-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="45420-196">Boolean</span></span>|<span data-ttu-id="45420-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="45420-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="45420-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45420-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45420-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="45420-199">roleScopeTagIds</span></span>|<span data-ttu-id="45420-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="45420-200">String collection</span></span>|<span data-ttu-id="45420-201">Lista de ids de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="45420-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="45420-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45420-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45420-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="45420-203">dependentAppCount</span></span>|<span data-ttu-id="45420-204">Int32</span><span class="sxs-lookup"><span data-stu-id="45420-204">Int32</span></span>|<span data-ttu-id="45420-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="45420-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="45420-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45420-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45420-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="45420-207">supersedingAppCount</span></span>|<span data-ttu-id="45420-208">Int32</span><span class="sxs-lookup"><span data-stu-id="45420-208">Int32</span></span>|<span data-ttu-id="45420-209">O número total de aplicativos que esse aplicativo sobressede direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="45420-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="45420-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45420-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="45420-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="45420-211">supersededAppCount</span></span>|<span data-ttu-id="45420-212">Int32</span><span class="sxs-lookup"><span data-stu-id="45420-212">Int32</span></span>|<span data-ttu-id="45420-213">O número total de aplicativos pelos quais esse aplicativo é, direta ou indiretamente, é suplido.</span><span class="sxs-lookup"><span data-stu-id="45420-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="45420-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="45420-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="45420-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="45420-215">Response</span></span>
<span data-ttu-id="45420-216">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45420-216">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45420-217">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45420-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="45420-218">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45420-218">Request</span></span>
<span data-ttu-id="45420-219">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45420-219">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 775

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
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
  "supersededAppCount": 2
}
```

### <a name="response"></a><span data-ttu-id="45420-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="45420-220">Response</span></span>
<span data-ttu-id="45420-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45420-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 947

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
  "id": "bf39e35d-e35d-bf39-5de3-39bf5de339bf",
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
  "supersededAppCount": 2
}
```




