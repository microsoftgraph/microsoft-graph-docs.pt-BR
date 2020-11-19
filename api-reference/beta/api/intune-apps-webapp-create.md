---
title: Criar webApp
description: Cria um novo objeto webApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4e8e47bffdfe5758cfb4bf32cf05c5174ad1130b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49247549"
---
# <a name="create-webapp"></a><span data-ttu-id="d4c29-103">Criar webApp</span><span class="sxs-lookup"><span data-stu-id="d4c29-103">Create webApp</span></span>

<span data-ttu-id="d4c29-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4c29-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4c29-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d4c29-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4c29-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d4c29-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4c29-107">Cria um novo objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="d4c29-107">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4c29-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d4c29-108">Prerequisites</span></span>
<span data-ttu-id="d4c29-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4c29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4c29-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4c29-111">Permission type</span></span>|<span data-ttu-id="d4c29-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d4c29-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4c29-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4c29-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4c29-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4c29-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d4c29-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4c29-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4c29-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4c29-116">Not supported.</span></span>|
|<span data-ttu-id="d4c29-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4c29-117">Application</span></span>|<span data-ttu-id="d4c29-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4c29-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4c29-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4c29-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d4c29-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4c29-120">Request headers</span></span>
|<span data-ttu-id="d4c29-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4c29-121">Header</span></span>|<span data-ttu-id="d4c29-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d4c29-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4c29-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4c29-123">Authorization</span></span>|<span data-ttu-id="d4c29-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4c29-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4c29-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d4c29-125">Accept</span></span>|<span data-ttu-id="d4c29-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4c29-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4c29-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4c29-127">Request body</span></span>
<span data-ttu-id="d4c29-128">No corpo da solicitação, forneça uma representação JSON do objeto webApp.</span><span class="sxs-lookup"><span data-stu-id="d4c29-128">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="d4c29-129">A tabela a seguir mostra as propriedades obrigatórias ao criar o webApp.</span><span class="sxs-lookup"><span data-stu-id="d4c29-129">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="d4c29-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4c29-130">Property</span></span>|<span data-ttu-id="d4c29-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4c29-131">Type</span></span>|<span data-ttu-id="d4c29-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4c29-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4c29-133">id</span><span class="sxs-lookup"><span data-stu-id="d4c29-133">id</span></span>|<span data-ttu-id="d4c29-134">String</span><span class="sxs-lookup"><span data-stu-id="d4c29-134">String</span></span>|<span data-ttu-id="d4c29-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d4c29-135">Key of the entity.</span></span> <span data-ttu-id="d4c29-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4c29-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c29-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d4c29-137">displayName</span></span>|<span data-ttu-id="d4c29-138">String</span><span class="sxs-lookup"><span data-stu-id="d4c29-138">String</span></span>|<span data-ttu-id="d4c29-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="d4c29-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d4c29-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4c29-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c29-141">description</span><span class="sxs-lookup"><span data-stu-id="d4c29-141">description</span></span>|<span data-ttu-id="d4c29-142">String</span><span class="sxs-lookup"><span data-stu-id="d4c29-142">String</span></span>|<span data-ttu-id="d4c29-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d4c29-143">The description of the app.</span></span> <span data-ttu-id="d4c29-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4c29-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c29-145">publicador</span><span class="sxs-lookup"><span data-stu-id="d4c29-145">publisher</span></span>|<span data-ttu-id="d4c29-146">String</span><span class="sxs-lookup"><span data-stu-id="d4c29-146">String</span></span>|<span data-ttu-id="d4c29-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d4c29-147">The publisher of the app.</span></span> <span data-ttu-id="d4c29-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4c29-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c29-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d4c29-149">largeIcon</span></span>|[<span data-ttu-id="d4c29-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d4c29-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d4c29-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="d4c29-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d4c29-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4c29-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c29-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4c29-153">createdDateTime</span></span>|<span data-ttu-id="d4c29-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4c29-154">DateTimeOffset</span></span>|<span data-ttu-id="d4c29-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d4c29-155">The date and time the app was created.</span></span> <span data-ttu-id="d4c29-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4c29-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c29-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4c29-157">lastModifiedDateTime</span></span>|<span data-ttu-id="d4c29-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4c29-158">DateTimeOffset</span></span>|<span data-ttu-id="d4c29-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d4c29-159">The date and time the app was last modified.</span></span> <span data-ttu-id="d4c29-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4c29-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c29-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d4c29-161">isFeatured</span></span>|<span data-ttu-id="d4c29-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4c29-162">Boolean</span></span>|<span data-ttu-id="d4c29-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4c29-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c29-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d4c29-164">privacyInformationUrl</span></span>|<span data-ttu-id="d4c29-165">String</span><span class="sxs-lookup"><span data-stu-id="d4c29-165">String</span></span>|<span data-ttu-id="d4c29-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="d4c29-166">The privacy statement Url.</span></span> <span data-ttu-id="d4c29-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4c29-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c29-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d4c29-168">informationUrl</span></span>|<span data-ttu-id="d4c29-169">String</span><span class="sxs-lookup"><span data-stu-id="d4c29-169">String</span></span>|<span data-ttu-id="d4c29-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="d4c29-170">The more information Url.</span></span> <span data-ttu-id="d4c29-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4c29-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c29-172">owner</span><span class="sxs-lookup"><span data-stu-id="d4c29-172">owner</span></span>|<span data-ttu-id="d4c29-173">String</span><span class="sxs-lookup"><span data-stu-id="d4c29-173">String</span></span>|<span data-ttu-id="d4c29-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="d4c29-174">The owner of the app.</span></span> <span data-ttu-id="d4c29-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4c29-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c29-176">developer</span><span class="sxs-lookup"><span data-stu-id="d4c29-176">developer</span></span>|<span data-ttu-id="d4c29-177">String</span><span class="sxs-lookup"><span data-stu-id="d4c29-177">String</span></span>|<span data-ttu-id="d4c29-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d4c29-178">The developer of the app.</span></span> <span data-ttu-id="d4c29-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4c29-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c29-180">notes</span><span class="sxs-lookup"><span data-stu-id="d4c29-180">notes</span></span>|<span data-ttu-id="d4c29-181">String</span><span class="sxs-lookup"><span data-stu-id="d4c29-181">String</span></span>|<span data-ttu-id="d4c29-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d4c29-182">Notes for the app.</span></span> <span data-ttu-id="d4c29-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4c29-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c29-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="d4c29-184">uploadState</span></span>|<span data-ttu-id="d4c29-185">Int32</span><span class="sxs-lookup"><span data-stu-id="d4c29-185">Int32</span></span>|<span data-ttu-id="d4c29-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="d4c29-186">The upload state.</span></span> <span data-ttu-id="d4c29-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="d4c29-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="d4c29-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4c29-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c29-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="d4c29-189">publishingState</span></span>|[<span data-ttu-id="d4c29-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d4c29-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d4c29-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d4c29-191">The publishing state for the app.</span></span> <span data-ttu-id="d4c29-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="d4c29-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d4c29-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d4c29-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="d4c29-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d4c29-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d4c29-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d4c29-195">isAssigned</span></span>|<span data-ttu-id="d4c29-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4c29-196">Boolean</span></span>|<span data-ttu-id="d4c29-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="d4c29-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="d4c29-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4c29-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c29-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d4c29-199">roleScopeTagIds</span></span>|<span data-ttu-id="d4c29-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4c29-200">String collection</span></span>|<span data-ttu-id="d4c29-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="d4c29-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="d4c29-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4c29-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c29-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="d4c29-203">dependentAppCount</span></span>|<span data-ttu-id="d4c29-204">Int32</span><span class="sxs-lookup"><span data-stu-id="d4c29-204">Int32</span></span>|<span data-ttu-id="d4c29-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="d4c29-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="d4c29-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4c29-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c29-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="d4c29-207">supersedingAppCount</span></span>|<span data-ttu-id="d4c29-208">Int32</span><span class="sxs-lookup"><span data-stu-id="d4c29-208">Int32</span></span>|<span data-ttu-id="d4c29-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="d4c29-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="d4c29-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4c29-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c29-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="d4c29-211">supersededAppCount</span></span>|<span data-ttu-id="d4c29-212">Int32</span><span class="sxs-lookup"><span data-stu-id="d4c29-212">Int32</span></span>|<span data-ttu-id="d4c29-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="d4c29-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="d4c29-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d4c29-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c29-215">appUrl</span><span class="sxs-lookup"><span data-stu-id="d4c29-215">appUrl</span></span>|<span data-ttu-id="d4c29-216">String</span><span class="sxs-lookup"><span data-stu-id="d4c29-216">String</span></span>|<span data-ttu-id="d4c29-217">A URL do aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="d4c29-217">The web app URL.</span></span>|
|<span data-ttu-id="d4c29-218">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="d4c29-218">useManagedBrowser</span></span>|<span data-ttu-id="d4c29-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4c29-219">Boolean</span></span>|<span data-ttu-id="d4c29-220">Se o navegador gerenciado deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="d4c29-220">Whether or not to use managed browser.</span></span> <span data-ttu-id="d4c29-221">Essa propriedade só é aplicável ao Android e ao IOS.</span><span class="sxs-lookup"><span data-stu-id="d4c29-221">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="d4c29-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4c29-222">Response</span></span>
<span data-ttu-id="d4c29-223">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [webApp](../resources/intune-apps-webapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4c29-223">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4c29-224">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4c29-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4c29-225">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4c29-225">Request</span></span>
<span data-ttu-id="d4c29-226">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4c29-226">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 836

{
  "@odata.type": "#microsoft.graph.webApp",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="d4c29-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4c29-227">Response</span></span>
<span data-ttu-id="d4c29-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4c29-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1008

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```




