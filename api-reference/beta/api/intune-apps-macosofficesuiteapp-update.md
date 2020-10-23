---
title: Atualizar macOSOfficeSuiteApp
description: Atualizar as propriedades de um objeto  macOSOfficeSuiteApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 17e269c5b36e15a9d486a067c8801f77efe9e0a4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48699755"
---
# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="ac04b-103">Atualizar macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="ac04b-103">Update macOSOfficeSuiteApp</span></span>

<span data-ttu-id="ac04b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac04b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ac04b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ac04b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac04b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ac04b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac04b-107">Atualizar as propriedades de um objeto [ macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="ac04b-107">Update the properties of a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac04b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ac04b-108">Prerequisites</span></span>
<span data-ttu-id="ac04b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac04b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac04b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac04b-111">Permission type</span></span>|<span data-ttu-id="ac04b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ac04b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac04b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac04b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ac04b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac04b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ac04b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac04b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac04b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac04b-116">Not supported.</span></span>|
|<span data-ttu-id="ac04b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac04b-117">Application</span></span>|<span data-ttu-id="ac04b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac04b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac04b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac04b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="ac04b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac04b-120">Request headers</span></span>
|<span data-ttu-id="ac04b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ac04b-121">Header</span></span>|<span data-ttu-id="ac04b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ac04b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac04b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac04b-123">Authorization</span></span>|<span data-ttu-id="ac04b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac04b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac04b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ac04b-125">Accept</span></span>|<span data-ttu-id="ac04b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ac04b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac04b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac04b-127">Request body</span></span>
<span data-ttu-id="ac04b-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="ac04b-128">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="ac04b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="ac04b-129">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="ac04b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac04b-130">Property</span></span>|<span data-ttu-id="ac04b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac04b-131">Type</span></span>|<span data-ttu-id="ac04b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac04b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac04b-133">id</span><span class="sxs-lookup"><span data-stu-id="ac04b-133">id</span></span>|<span data-ttu-id="ac04b-134">String</span><span class="sxs-lookup"><span data-stu-id="ac04b-134">String</span></span>|<span data-ttu-id="ac04b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ac04b-135">Key of the entity.</span></span> <span data-ttu-id="ac04b-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac04b-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac04b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ac04b-137">displayName</span></span>|<span data-ttu-id="ac04b-138">String</span><span class="sxs-lookup"><span data-stu-id="ac04b-138">String</span></span>|<span data-ttu-id="ac04b-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ac04b-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ac04b-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac04b-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac04b-141">description</span><span class="sxs-lookup"><span data-stu-id="ac04b-141">description</span></span>|<span data-ttu-id="ac04b-142">String</span><span class="sxs-lookup"><span data-stu-id="ac04b-142">String</span></span>|<span data-ttu-id="ac04b-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ac04b-143">The description of the app.</span></span> <span data-ttu-id="ac04b-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac04b-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac04b-145">publicador</span><span class="sxs-lookup"><span data-stu-id="ac04b-145">publisher</span></span>|<span data-ttu-id="ac04b-146">String</span><span class="sxs-lookup"><span data-stu-id="ac04b-146">String</span></span>|<span data-ttu-id="ac04b-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ac04b-147">The publisher of the app.</span></span> <span data-ttu-id="ac04b-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac04b-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac04b-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ac04b-149">largeIcon</span></span>|[<span data-ttu-id="ac04b-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ac04b-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ac04b-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="ac04b-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ac04b-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac04b-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac04b-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ac04b-153">createdDateTime</span></span>|<span data-ttu-id="ac04b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac04b-154">DateTimeOffset</span></span>|<span data-ttu-id="ac04b-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ac04b-155">The date and time the app was created.</span></span> <span data-ttu-id="ac04b-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac04b-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac04b-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac04b-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ac04b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac04b-158">DateTimeOffset</span></span>|<span data-ttu-id="ac04b-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ac04b-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ac04b-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac04b-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac04b-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ac04b-161">isFeatured</span></span>|<span data-ttu-id="ac04b-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac04b-162">Boolean</span></span>|<span data-ttu-id="ac04b-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac04b-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac04b-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ac04b-164">privacyInformationUrl</span></span>|<span data-ttu-id="ac04b-165">String</span><span class="sxs-lookup"><span data-stu-id="ac04b-165">String</span></span>|<span data-ttu-id="ac04b-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="ac04b-166">The privacy statement Url.</span></span> <span data-ttu-id="ac04b-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac04b-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac04b-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ac04b-168">informationUrl</span></span>|<span data-ttu-id="ac04b-169">String</span><span class="sxs-lookup"><span data-stu-id="ac04b-169">String</span></span>|<span data-ttu-id="ac04b-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="ac04b-170">The more information Url.</span></span> <span data-ttu-id="ac04b-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac04b-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac04b-172">owner</span><span class="sxs-lookup"><span data-stu-id="ac04b-172">owner</span></span>|<span data-ttu-id="ac04b-173">String</span><span class="sxs-lookup"><span data-stu-id="ac04b-173">String</span></span>|<span data-ttu-id="ac04b-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ac04b-174">The owner of the app.</span></span> <span data-ttu-id="ac04b-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac04b-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac04b-176">developer</span><span class="sxs-lookup"><span data-stu-id="ac04b-176">developer</span></span>|<span data-ttu-id="ac04b-177">String</span><span class="sxs-lookup"><span data-stu-id="ac04b-177">String</span></span>|<span data-ttu-id="ac04b-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ac04b-178">The developer of the app.</span></span> <span data-ttu-id="ac04b-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac04b-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac04b-180">notes</span><span class="sxs-lookup"><span data-stu-id="ac04b-180">notes</span></span>|<span data-ttu-id="ac04b-181">String</span><span class="sxs-lookup"><span data-stu-id="ac04b-181">String</span></span>|<span data-ttu-id="ac04b-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ac04b-182">Notes for the app.</span></span> <span data-ttu-id="ac04b-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac04b-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac04b-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ac04b-184">uploadState</span></span>|<span data-ttu-id="ac04b-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ac04b-185">Int32</span></span>|<span data-ttu-id="ac04b-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="ac04b-186">The upload state.</span></span> <span data-ttu-id="ac04b-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="ac04b-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="ac04b-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac04b-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac04b-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="ac04b-189">publishingState</span></span>|[<span data-ttu-id="ac04b-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ac04b-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ac04b-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ac04b-191">The publishing state for the app.</span></span> <span data-ttu-id="ac04b-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="ac04b-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ac04b-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ac04b-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="ac04b-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ac04b-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ac04b-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ac04b-195">isAssigned</span></span>|<span data-ttu-id="ac04b-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac04b-196">Boolean</span></span>|<span data-ttu-id="ac04b-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="ac04b-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ac04b-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac04b-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac04b-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ac04b-199">roleScopeTagIds</span></span>|<span data-ttu-id="ac04b-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac04b-200">String collection</span></span>|<span data-ttu-id="ac04b-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="ac04b-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ac04b-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac04b-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac04b-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="ac04b-203">dependentAppCount</span></span>|<span data-ttu-id="ac04b-204">Int32</span><span class="sxs-lookup"><span data-stu-id="ac04b-204">Int32</span></span>|<span data-ttu-id="ac04b-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="ac04b-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="ac04b-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac04b-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac04b-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="ac04b-207">supersedingAppCount</span></span>|<span data-ttu-id="ac04b-208">Int32</span><span class="sxs-lookup"><span data-stu-id="ac04b-208">Int32</span></span>|<span data-ttu-id="ac04b-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="ac04b-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="ac04b-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac04b-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ac04b-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="ac04b-211">supersededAppCount</span></span>|<span data-ttu-id="ac04b-212">Int32</span><span class="sxs-lookup"><span data-stu-id="ac04b-212">Int32</span></span>|<span data-ttu-id="ac04b-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="ac04b-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="ac04b-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ac04b-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ac04b-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac04b-215">Response</span></span>
<span data-ttu-id="ac04b-216">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac04b-216">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac04b-217">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac04b-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac04b-218">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac04b-218">Request</span></span>
<span data-ttu-id="ac04b-219">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac04b-219">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ac04b-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac04b-220">Response</span></span>
<span data-ttu-id="ac04b-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac04b-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





