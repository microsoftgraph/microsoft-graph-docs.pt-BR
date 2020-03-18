---
title: Criar officeSuiteApp
description: Criar um novo objeto officeSuiteApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 548012134a88d6d3482e5eef3f256173c76b13e1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761108"
---
# <a name="create-officesuiteapp"></a><span data-ttu-id="f4e71-103">Criar officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="f4e71-103">Create officeSuiteApp</span></span>

> <span data-ttu-id="f4e71-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f4e71-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4e71-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4e71-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4e71-106">Criar um novo objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) .</span><span class="sxs-lookup"><span data-stu-id="f4e71-106">Create a new [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4e71-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f4e71-107">Prerequisites</span></span>
<span data-ttu-id="f4e71-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4e71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4e71-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4e71-110">Permission type</span></span>|<span data-ttu-id="f4e71-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f4e71-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4e71-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4e71-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4e71-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4e71-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f4e71-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4e71-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4e71-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4e71-115">Not supported.</span></span>|
|<span data-ttu-id="f4e71-116">Application</span><span class="sxs-lookup"><span data-stu-id="f4e71-116">Application</span></span>|<span data-ttu-id="f4e71-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4e71-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4e71-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4e71-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f4e71-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4e71-119">Request headers</span></span>
|<span data-ttu-id="f4e71-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f4e71-120">Header</span></span>|<span data-ttu-id="f4e71-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f4e71-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4e71-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4e71-122">Authorization</span></span>|<span data-ttu-id="f4e71-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4e71-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4e71-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f4e71-124">Accept</span></span>|<span data-ttu-id="f4e71-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4e71-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4e71-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4e71-126">Request body</span></span>
<span data-ttu-id="f4e71-127">No corpo da solicitação, forneça uma representação JSON do objeto officeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="f4e71-127">In the request body, supply a JSON representation for the officeSuiteApp object.</span></span>

<span data-ttu-id="f4e71-128">A tabela a seguir mostra as propriedades que são necessárias ao criar officeSuiteApp.</span><span class="sxs-lookup"><span data-stu-id="f4e71-128">The following table shows the properties that are required when you create the officeSuiteApp.</span></span>

|<span data-ttu-id="f4e71-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4e71-129">Property</span></span>|<span data-ttu-id="f4e71-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4e71-130">Type</span></span>|<span data-ttu-id="f4e71-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4e71-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4e71-132">id</span><span class="sxs-lookup"><span data-stu-id="f4e71-132">id</span></span>|<span data-ttu-id="f4e71-133">String</span><span class="sxs-lookup"><span data-stu-id="f4e71-133">String</span></span>|<span data-ttu-id="f4e71-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f4e71-134">Key of the entity.</span></span> <span data-ttu-id="f4e71-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4e71-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f4e71-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f4e71-136">displayName</span></span>|<span data-ttu-id="f4e71-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4e71-137">String</span></span>|<span data-ttu-id="f4e71-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f4e71-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f4e71-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4e71-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f4e71-140">description</span><span class="sxs-lookup"><span data-stu-id="f4e71-140">description</span></span>|<span data-ttu-id="f4e71-141">String</span><span class="sxs-lookup"><span data-stu-id="f4e71-141">String</span></span>|<span data-ttu-id="f4e71-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4e71-142">The description of the app.</span></span> <span data-ttu-id="f4e71-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4e71-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f4e71-144">publicador</span><span class="sxs-lookup"><span data-stu-id="f4e71-144">publisher</span></span>|<span data-ttu-id="f4e71-145">String</span><span class="sxs-lookup"><span data-stu-id="f4e71-145">String</span></span>|<span data-ttu-id="f4e71-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4e71-146">The publisher of the app.</span></span> <span data-ttu-id="f4e71-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4e71-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f4e71-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f4e71-148">largeIcon</span></span>|[<span data-ttu-id="f4e71-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f4e71-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f4e71-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="f4e71-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f4e71-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4e71-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f4e71-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4e71-152">createdDateTime</span></span>|<span data-ttu-id="f4e71-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4e71-153">DateTimeOffset</span></span>|<span data-ttu-id="f4e71-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4e71-154">The date and time the app was created.</span></span> <span data-ttu-id="f4e71-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4e71-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f4e71-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4e71-156">lastModifiedDateTime</span></span>|<span data-ttu-id="f4e71-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4e71-157">DateTimeOffset</span></span>|<span data-ttu-id="f4e71-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f4e71-158">The date and time the app was last modified.</span></span> <span data-ttu-id="f4e71-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4e71-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f4e71-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f4e71-160">isFeatured</span></span>|<span data-ttu-id="f4e71-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4e71-161">Boolean</span></span>|<span data-ttu-id="f4e71-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4e71-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f4e71-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f4e71-163">privacyInformationUrl</span></span>|<span data-ttu-id="f4e71-164">String</span><span class="sxs-lookup"><span data-stu-id="f4e71-164">String</span></span>|<span data-ttu-id="f4e71-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="f4e71-165">The privacy statement Url.</span></span> <span data-ttu-id="f4e71-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4e71-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f4e71-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f4e71-167">informationUrl</span></span>|<span data-ttu-id="f4e71-168">String</span><span class="sxs-lookup"><span data-stu-id="f4e71-168">String</span></span>|<span data-ttu-id="f4e71-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="f4e71-169">The more information Url.</span></span> <span data-ttu-id="f4e71-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4e71-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f4e71-171">owner</span><span class="sxs-lookup"><span data-stu-id="f4e71-171">owner</span></span>|<span data-ttu-id="f4e71-172">String</span><span class="sxs-lookup"><span data-stu-id="f4e71-172">String</span></span>|<span data-ttu-id="f4e71-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f4e71-173">The owner of the app.</span></span> <span data-ttu-id="f4e71-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4e71-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f4e71-175">developer</span><span class="sxs-lookup"><span data-stu-id="f4e71-175">developer</span></span>|<span data-ttu-id="f4e71-176">String</span><span class="sxs-lookup"><span data-stu-id="f4e71-176">String</span></span>|<span data-ttu-id="f4e71-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4e71-177">The developer of the app.</span></span> <span data-ttu-id="f4e71-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4e71-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f4e71-179">notes</span><span class="sxs-lookup"><span data-stu-id="f4e71-179">notes</span></span>|<span data-ttu-id="f4e71-180">String</span><span class="sxs-lookup"><span data-stu-id="f4e71-180">String</span></span>|<span data-ttu-id="f4e71-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4e71-181">Notes for the app.</span></span> <span data-ttu-id="f4e71-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4e71-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f4e71-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="f4e71-183">uploadState</span></span>|<span data-ttu-id="f4e71-184">Int32</span><span class="sxs-lookup"><span data-stu-id="f4e71-184">Int32</span></span>|<span data-ttu-id="f4e71-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="f4e71-185">The upload state.</span></span> <span data-ttu-id="f4e71-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4e71-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f4e71-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="f4e71-187">publishingState</span></span>|[<span data-ttu-id="f4e71-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f4e71-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f4e71-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4e71-189">The publishing state for the app.</span></span> <span data-ttu-id="f4e71-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="f4e71-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f4e71-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f4e71-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="f4e71-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f4e71-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f4e71-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f4e71-193">isAssigned</span></span>|<span data-ttu-id="f4e71-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4e71-194">Boolean</span></span>|<span data-ttu-id="f4e71-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="f4e71-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f4e71-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4e71-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f4e71-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f4e71-197">roleScopeTagIds</span></span>|<span data-ttu-id="f4e71-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4e71-198">String collection</span></span>|<span data-ttu-id="f4e71-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="f4e71-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f4e71-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4e71-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f4e71-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="f4e71-201">dependentAppCount</span></span>|<span data-ttu-id="f4e71-202">Int32</span><span class="sxs-lookup"><span data-stu-id="f4e71-202">Int32</span></span>|<span data-ttu-id="f4e71-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="f4e71-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="f4e71-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4e71-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f4e71-205">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="f4e71-205">autoAcceptEula</span></span>|<span data-ttu-id="f4e71-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4e71-206">Boolean</span></span>|<span data-ttu-id="f4e71-207">O valor para aceitar o EULA automaticamente no dispositivo do usuário.</span><span class="sxs-lookup"><span data-stu-id="f4e71-207">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="f4e71-208">productIds</span><span class="sxs-lookup"><span data-stu-id="f4e71-208">productIds</span></span>|<span data-ttu-id="f4e71-209">coleção [officeProductId](../resources/intune-apps-officeproductid.md)</span><span class="sxs-lookup"><span data-stu-id="f4e71-209">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="f4e71-210">As IDs de produto que representam a SKU do pacote do office365.</span><span class="sxs-lookup"><span data-stu-id="f4e71-210">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="f4e71-211">Os valores possíveis são: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span><span class="sxs-lookup"><span data-stu-id="f4e71-211">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="f4e71-212">excludedApps</span><span class="sxs-lookup"><span data-stu-id="f4e71-212">excludedApps</span></span>|[<span data-ttu-id="f4e71-213">excludedApps</span><span class="sxs-lookup"><span data-stu-id="f4e71-213">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="f4e71-214">A propriedade para representar os aplicativos que são excluídos da ID de produto do Office365 selecionado.</span><span class="sxs-lookup"><span data-stu-id="f4e71-214">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="f4e71-215">Propriedades usesharedcomputeractivation</span><span class="sxs-lookup"><span data-stu-id="f4e71-215">useSharedComputerActivation</span></span>|<span data-ttu-id="f4e71-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4e71-216">Boolean</span></span>|<span data-ttu-id="f4e71-217">A propriedade que representa se a ativação de computador compartilhado é usada não para o pacote de aplicativos do office365.</span><span class="sxs-lookup"><span data-stu-id="f4e71-217">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="f4e71-218">updateChannel</span><span class="sxs-lookup"><span data-stu-id="f4e71-218">updateChannel</span></span>|[<span data-ttu-id="f4e71-219">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="f4e71-219">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="f4e71-220">A propriedade para representar o canal de atualização do office365.</span><span class="sxs-lookup"><span data-stu-id="f4e71-220">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="f4e71-221">Os valores possíveis são: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span><span class="sxs-lookup"><span data-stu-id="f4e71-221">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="f4e71-222">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="f4e71-222">officePlatformArchitecture</span></span>|[<span data-ttu-id="f4e71-223">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="f4e71-223">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="f4e71-224">A propriedade para representar a versão do pacote de aplicativos do office365.</span><span class="sxs-lookup"><span data-stu-id="f4e71-224">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="f4e71-225">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="f4e71-225">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="f4e71-226">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="f4e71-226">localesToInstall</span></span>|<span data-ttu-id="f4e71-227">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4e71-227">String collection</span></span>|<span data-ttu-id="f4e71-228">A propriedade para representar os locais que são instalados quando os aplicativos do Office365 estão instalados.</span><span class="sxs-lookup"><span data-stu-id="f4e71-228">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="f4e71-229">Ele usa RFC 6033 padrão.</span><span class="sxs-lookup"><span data-stu-id="f4e71-229">It uses standard RFC 6033.</span></span> <span data-ttu-id="f4e71-230">Refhttps://technet.microsoft.com/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="f4e71-230">Ref: https://technet.microsoft.com/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="f4e71-231">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="f4e71-231">installProgressDisplayLevel</span></span>|[<span data-ttu-id="f4e71-232">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="f4e71-232">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="f4e71-233">Para especificar o nível de exibição da interface do usuário da configuração de progresso da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f4e71-233">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="f4e71-234">Os valores possíveis são: `none` e `full`.</span><span class="sxs-lookup"><span data-stu-id="f4e71-234">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="f4e71-235">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="f4e71-235">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="f4e71-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4e71-236">Boolean</span></span>|<span data-ttu-id="f4e71-237">A propriedade para determinar se deve desinstalar o Office MSI existente se um pacote de aplicativos do Office365 for implantado no dispositivo ou não.</span><span class="sxs-lookup"><span data-stu-id="f4e71-237">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="f4e71-238">targetVersion</span><span class="sxs-lookup"><span data-stu-id="f4e71-238">targetVersion</span></span>|<span data-ttu-id="f4e71-239">String</span><span class="sxs-lookup"><span data-stu-id="f4e71-239">String</span></span>|<span data-ttu-id="f4e71-240">A propriedade para representar a versão de destino específica para o pacote de aplicativos do Office365 que deve permanecer implantado nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f4e71-240">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="f4e71-241">updateVersion</span><span class="sxs-lookup"><span data-stu-id="f4e71-241">updateVersion</span></span>|<span data-ttu-id="f4e71-242">String</span><span class="sxs-lookup"><span data-stu-id="f4e71-242">String</span></span>|<span data-ttu-id="f4e71-243">A propriedade para representar a versão de atualização na qual a versão de destino específica está disponível para o pacote de aplicativos do office365.</span><span class="sxs-lookup"><span data-stu-id="f4e71-243">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="f4e71-244">officeConfigurationXml</span><span class="sxs-lookup"><span data-stu-id="f4e71-244">officeConfigurationXml</span></span>|<span data-ttu-id="f4e71-245">Binária</span><span class="sxs-lookup"><span data-stu-id="f4e71-245">Binary</span></span>|<span data-ttu-id="f4e71-246">A propriedade para representar o arquivo de configuração XML que pode ser especificado para aplicativos do Office ProPlus.</span><span class="sxs-lookup"><span data-stu-id="f4e71-246">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="f4e71-247">Tem precedência sobre todas as outras propriedades.</span><span class="sxs-lookup"><span data-stu-id="f4e71-247">Takes precedence over all other properties.</span></span> <span data-ttu-id="f4e71-248">Quando presente, o arquivo de configuração XML será usado para criar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4e71-248">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="f4e71-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4e71-249">Response</span></span>
<span data-ttu-id="f4e71-250">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4e71-250">If successful, this method returns a `201 Created` response code and a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4e71-251">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4e71-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4e71-252">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4e71-252">Request</span></span>
<span data-ttu-id="f4e71-253">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4e71-253">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1599

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
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
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

### <a name="response"></a><span data-ttu-id="f4e71-254">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4e71-254">Response</span></span>
<span data-ttu-id="f4e71-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4e71-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1771

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
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
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




