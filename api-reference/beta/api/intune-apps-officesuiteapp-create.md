---
title: Criar officeSuiteApp
description: Criar um novo objeto officeSuiteApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f6079e4b0b5f8dccade2f244d752a790a2ce2506
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47976946"
---
# <a name="create-officesuiteapp"></a><span data-ttu-id="53e5d-103">Criar officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="53e5d-103">Create officeSuiteApp</span></span>

<span data-ttu-id="53e5d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53e5d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53e5d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="53e5d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53e5d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="53e5d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53e5d-107">Criar um novo objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="53e5d-107">Create a new [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53e5d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="53e5d-108">Prerequisites</span></span>
<span data-ttu-id="53e5d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53e5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53e5d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53e5d-111">Permission type</span></span>|<span data-ttu-id="53e5d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="53e5d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53e5d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53e5d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53e5d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53e5d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="53e5d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53e5d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53e5d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53e5d-116">Not supported.</span></span>|
|<span data-ttu-id="53e5d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53e5d-117">Application</span></span>|<span data-ttu-id="53e5d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53e5d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53e5d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53e5d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="53e5d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53e5d-120">Request headers</span></span>
|<span data-ttu-id="53e5d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="53e5d-121">Header</span></span>|<span data-ttu-id="53e5d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="53e5d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53e5d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="53e5d-123">Authorization</span></span>|<span data-ttu-id="53e5d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53e5d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53e5d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="53e5d-125">Accept</span></span>|<span data-ttu-id="53e5d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53e5d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53e5d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53e5d-127">Request body</span></span>
<span data-ttu-id="53e5d-128">No corpo da solicitação, forneça uma representação JSON do objeto officeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="53e5d-128">In the request body, supply a JSON representation for the officeSuiteApp object.</span></span>

<span data-ttu-id="53e5d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar officeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="53e5d-129">The following table shows the properties that are required when you create the officeSuiteApp.</span></span>

|<span data-ttu-id="53e5d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53e5d-130">Property</span></span>|<span data-ttu-id="53e5d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="53e5d-131">Type</span></span>|<span data-ttu-id="53e5d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="53e5d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53e5d-133">id</span><span class="sxs-lookup"><span data-stu-id="53e5d-133">id</span></span>|<span data-ttu-id="53e5d-134">String</span><span class="sxs-lookup"><span data-stu-id="53e5d-134">String</span></span>|<span data-ttu-id="53e5d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="53e5d-135">Key of the entity.</span></span> <span data-ttu-id="53e5d-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53e5d-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53e5d-137">displayName</span><span class="sxs-lookup"><span data-stu-id="53e5d-137">displayName</span></span>|<span data-ttu-id="53e5d-138">String</span><span class="sxs-lookup"><span data-stu-id="53e5d-138">String</span></span>|<span data-ttu-id="53e5d-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="53e5d-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="53e5d-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53e5d-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53e5d-141">description</span><span class="sxs-lookup"><span data-stu-id="53e5d-141">description</span></span>|<span data-ttu-id="53e5d-142">String</span><span class="sxs-lookup"><span data-stu-id="53e5d-142">String</span></span>|<span data-ttu-id="53e5d-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53e5d-143">The description of the app.</span></span> <span data-ttu-id="53e5d-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53e5d-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53e5d-145">publicador</span><span class="sxs-lookup"><span data-stu-id="53e5d-145">publisher</span></span>|<span data-ttu-id="53e5d-146">String</span><span class="sxs-lookup"><span data-stu-id="53e5d-146">String</span></span>|<span data-ttu-id="53e5d-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53e5d-147">The publisher of the app.</span></span> <span data-ttu-id="53e5d-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53e5d-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53e5d-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="53e5d-149">largeIcon</span></span>|[<span data-ttu-id="53e5d-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="53e5d-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="53e5d-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="53e5d-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="53e5d-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53e5d-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53e5d-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="53e5d-153">createdDateTime</span></span>|<span data-ttu-id="53e5d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53e5d-154">DateTimeOffset</span></span>|<span data-ttu-id="53e5d-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53e5d-155">The date and time the app was created.</span></span> <span data-ttu-id="53e5d-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53e5d-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53e5d-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53e5d-157">lastModifiedDateTime</span></span>|<span data-ttu-id="53e5d-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53e5d-158">DateTimeOffset</span></span>|<span data-ttu-id="53e5d-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="53e5d-159">The date and time the app was last modified.</span></span> <span data-ttu-id="53e5d-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53e5d-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53e5d-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="53e5d-161">isFeatured</span></span>|<span data-ttu-id="53e5d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="53e5d-162">Boolean</span></span>|<span data-ttu-id="53e5d-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53e5d-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53e5d-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="53e5d-164">privacyInformationUrl</span></span>|<span data-ttu-id="53e5d-165">String</span><span class="sxs-lookup"><span data-stu-id="53e5d-165">String</span></span>|<span data-ttu-id="53e5d-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="53e5d-166">The privacy statement Url.</span></span> <span data-ttu-id="53e5d-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53e5d-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53e5d-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="53e5d-168">informationUrl</span></span>|<span data-ttu-id="53e5d-169">String</span><span class="sxs-lookup"><span data-stu-id="53e5d-169">String</span></span>|<span data-ttu-id="53e5d-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="53e5d-170">The more information Url.</span></span> <span data-ttu-id="53e5d-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53e5d-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53e5d-172">proprietário</span><span class="sxs-lookup"><span data-stu-id="53e5d-172">owner</span></span>|<span data-ttu-id="53e5d-173">String</span><span class="sxs-lookup"><span data-stu-id="53e5d-173">String</span></span>|<span data-ttu-id="53e5d-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="53e5d-174">The owner of the app.</span></span> <span data-ttu-id="53e5d-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53e5d-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53e5d-176">developer</span><span class="sxs-lookup"><span data-stu-id="53e5d-176">developer</span></span>|<span data-ttu-id="53e5d-177">String</span><span class="sxs-lookup"><span data-stu-id="53e5d-177">String</span></span>|<span data-ttu-id="53e5d-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53e5d-178">The developer of the app.</span></span> <span data-ttu-id="53e5d-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53e5d-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53e5d-180">notes</span><span class="sxs-lookup"><span data-stu-id="53e5d-180">notes</span></span>|<span data-ttu-id="53e5d-181">String</span><span class="sxs-lookup"><span data-stu-id="53e5d-181">String</span></span>|<span data-ttu-id="53e5d-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53e5d-182">Notes for the app.</span></span> <span data-ttu-id="53e5d-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53e5d-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53e5d-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="53e5d-184">uploadState</span></span>|<span data-ttu-id="53e5d-185">Int32</span><span class="sxs-lookup"><span data-stu-id="53e5d-185">Int32</span></span>|<span data-ttu-id="53e5d-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="53e5d-186">The upload state.</span></span> <span data-ttu-id="53e5d-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="53e5d-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="53e5d-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53e5d-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53e5d-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="53e5d-189">publishingState</span></span>|[<span data-ttu-id="53e5d-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="53e5d-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="53e5d-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53e5d-191">The publishing state for the app.</span></span> <span data-ttu-id="53e5d-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="53e5d-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="53e5d-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53e5d-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="53e5d-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="53e5d-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="53e5d-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="53e5d-195">isAssigned</span></span>|<span data-ttu-id="53e5d-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="53e5d-196">Boolean</span></span>|<span data-ttu-id="53e5d-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="53e5d-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="53e5d-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53e5d-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53e5d-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="53e5d-199">roleScopeTagIds</span></span>|<span data-ttu-id="53e5d-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="53e5d-200">String collection</span></span>|<span data-ttu-id="53e5d-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="53e5d-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="53e5d-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53e5d-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53e5d-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="53e5d-203">dependentAppCount</span></span>|<span data-ttu-id="53e5d-204">Int32</span><span class="sxs-lookup"><span data-stu-id="53e5d-204">Int32</span></span>|<span data-ttu-id="53e5d-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="53e5d-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="53e5d-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53e5d-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53e5d-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="53e5d-207">supersedingAppCount</span></span>|<span data-ttu-id="53e5d-208">Int32</span><span class="sxs-lookup"><span data-stu-id="53e5d-208">Int32</span></span>|<span data-ttu-id="53e5d-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="53e5d-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="53e5d-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53e5d-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53e5d-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="53e5d-211">supersededAppCount</span></span>|<span data-ttu-id="53e5d-212">Int32</span><span class="sxs-lookup"><span data-stu-id="53e5d-212">Int32</span></span>|<span data-ttu-id="53e5d-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="53e5d-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="53e5d-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53e5d-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53e5d-215">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="53e5d-215">autoAcceptEula</span></span>|<span data-ttu-id="53e5d-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="53e5d-216">Boolean</span></span>|<span data-ttu-id="53e5d-217">O valor para aceitar o EULA automaticamente no dispositivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="53e5d-217">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="53e5d-218">productIds</span><span class="sxs-lookup"><span data-stu-id="53e5d-218">productIds</span></span>|<span data-ttu-id="53e5d-219">coleção [officeProductId](../resources/intune-apps-officeproductid.md)</span><span class="sxs-lookup"><span data-stu-id="53e5d-219">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="53e5d-220">As IDs de produto que representam a SKU do pacote do office365.</span><span class="sxs-lookup"><span data-stu-id="53e5d-220">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="53e5d-221">Os valores possíveis são: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span><span class="sxs-lookup"><span data-stu-id="53e5d-221">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="53e5d-222">excludedApps</span><span class="sxs-lookup"><span data-stu-id="53e5d-222">excludedApps</span></span>|[<span data-ttu-id="53e5d-223">excludedApps</span><span class="sxs-lookup"><span data-stu-id="53e5d-223">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="53e5d-224">A propriedade para representar os aplicativos que são excluídos da ID de produto do Office365 selecionado.</span><span class="sxs-lookup"><span data-stu-id="53e5d-224">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="53e5d-225">Propriedades usesharedcomputeractivation</span><span class="sxs-lookup"><span data-stu-id="53e5d-225">useSharedComputerActivation</span></span>|<span data-ttu-id="53e5d-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="53e5d-226">Boolean</span></span>|<span data-ttu-id="53e5d-227">A propriedade que representa se a ativação de computador compartilhado é usada não para o pacote de aplicativos do office365.</span><span class="sxs-lookup"><span data-stu-id="53e5d-227">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="53e5d-228">updateChannel</span><span class="sxs-lookup"><span data-stu-id="53e5d-228">updateChannel</span></span>|[<span data-ttu-id="53e5d-229">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="53e5d-229">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="53e5d-230">A propriedade para representar o canal de atualização do office365.</span><span class="sxs-lookup"><span data-stu-id="53e5d-230">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="53e5d-231">Os possíveis valores são: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`, `monthlyEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="53e5d-231">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`, `monthlyEnterprise`.</span></span>|
|<span data-ttu-id="53e5d-232">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="53e5d-232">officePlatformArchitecture</span></span>|[<span data-ttu-id="53e5d-233">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="53e5d-233">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="53e5d-234">A propriedade para representar a versão do pacote de aplicativos do office365.</span><span class="sxs-lookup"><span data-stu-id="53e5d-234">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="53e5d-235">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="53e5d-235">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="53e5d-236">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="53e5d-236">localesToInstall</span></span>|<span data-ttu-id="53e5d-237">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="53e5d-237">String collection</span></span>|<span data-ttu-id="53e5d-238">A propriedade para representar os locais que são instalados quando os aplicativos do Office365 estão instalados.</span><span class="sxs-lookup"><span data-stu-id="53e5d-238">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="53e5d-239">Ele usa RFC 6033 padrão.</span><span class="sxs-lookup"><span data-stu-id="53e5d-239">It uses standard RFC 6033.</span></span> <span data-ttu-id="53e5d-240">Ref https://technet.microsoft.com/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="53e5d-240">Ref: https://technet.microsoft.com/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="53e5d-241">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="53e5d-241">installProgressDisplayLevel</span></span>|[<span data-ttu-id="53e5d-242">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="53e5d-242">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="53e5d-243">Para especificar o nível de exibição da interface do usuário da configuração de progresso da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="53e5d-243">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="53e5d-244">Os valores possíveis são: `none` e `full`.</span><span class="sxs-lookup"><span data-stu-id="53e5d-244">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="53e5d-245">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="53e5d-245">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="53e5d-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="53e5d-246">Boolean</span></span>|<span data-ttu-id="53e5d-247">A propriedade para determinar se deve desinstalar o Office MSI existente se um pacote de aplicativos do Office365 for implantado no dispositivo ou não.</span><span class="sxs-lookup"><span data-stu-id="53e5d-247">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="53e5d-248">targetVersion</span><span class="sxs-lookup"><span data-stu-id="53e5d-248">targetVersion</span></span>|<span data-ttu-id="53e5d-249">String</span><span class="sxs-lookup"><span data-stu-id="53e5d-249">String</span></span>|<span data-ttu-id="53e5d-250">A propriedade para representar a versão de destino específica para o pacote de aplicativos do Office365 que deve permanecer implantado nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="53e5d-250">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="53e5d-251">updateVersion</span><span class="sxs-lookup"><span data-stu-id="53e5d-251">updateVersion</span></span>|<span data-ttu-id="53e5d-252">String</span><span class="sxs-lookup"><span data-stu-id="53e5d-252">String</span></span>|<span data-ttu-id="53e5d-253">A propriedade para representar a versão de atualização na qual a versão de destino específica está disponível para o pacote de aplicativos do office365.</span><span class="sxs-lookup"><span data-stu-id="53e5d-253">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="53e5d-254">officeConfigurationXml</span><span class="sxs-lookup"><span data-stu-id="53e5d-254">officeConfigurationXml</span></span>|<span data-ttu-id="53e5d-255">Binária</span><span class="sxs-lookup"><span data-stu-id="53e5d-255">Binary</span></span>|<span data-ttu-id="53e5d-256">A propriedade para representar o arquivo de configuração XML que pode ser especificado para aplicativos do Office ProPlus.</span><span class="sxs-lookup"><span data-stu-id="53e5d-256">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="53e5d-257">Tem precedência sobre todas as outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="53e5d-257">Takes precedence over all other properties.</span></span> <span data-ttu-id="53e5d-258">Quando presente, o arquivo de configuração XML será usado para criar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53e5d-258">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="53e5d-259">Resposta</span><span class="sxs-lookup"><span data-stu-id="53e5d-259">Response</span></span>
<span data-ttu-id="53e5d-260">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53e5d-260">If successful, this method returns a `201 Created` response code and a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53e5d-261">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53e5d-261">Example</span></span>

### <a name="request"></a><span data-ttu-id="53e5d-262">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53e5d-262">Request</span></span>
<span data-ttu-id="53e5d-263">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53e5d-263">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="53e5d-264">Resposta</span><span class="sxs-lookup"><span data-stu-id="53e5d-264">Response</span></span>
<span data-ttu-id="53e5d-p127">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53e5d-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






