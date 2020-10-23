---
title: Atualizar webApp
description: Atualiza as propriedades de um objeto webApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2dc91c4edc73a8b3b3b20f1c0df3e20d4aed1a91
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694820"
---
# <a name="update-webapp"></a><span data-ttu-id="33e00-103">Atualizar webApp</span><span class="sxs-lookup"><span data-stu-id="33e00-103">Update webApp</span></span>

<span data-ttu-id="33e00-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33e00-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="33e00-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="33e00-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33e00-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="33e00-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33e00-107">Atualiza as propriedades de um objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="33e00-107">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33e00-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="33e00-108">Prerequisites</span></span>
<span data-ttu-id="33e00-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33e00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33e00-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33e00-111">Permission type</span></span>|<span data-ttu-id="33e00-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="33e00-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33e00-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33e00-113">Delegated (work or school account)</span></span>|<span data-ttu-id="33e00-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33e00-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="33e00-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33e00-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33e00-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="33e00-116">Not supported.</span></span>|
|<span data-ttu-id="33e00-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33e00-117">Application</span></span>|<span data-ttu-id="33e00-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33e00-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="33e00-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33e00-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="33e00-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33e00-120">Request headers</span></span>
|<span data-ttu-id="33e00-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="33e00-121">Header</span></span>|<span data-ttu-id="33e00-122">Valor</span><span class="sxs-lookup"><span data-stu-id="33e00-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33e00-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="33e00-123">Authorization</span></span>|<span data-ttu-id="33e00-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33e00-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33e00-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="33e00-125">Accept</span></span>|<span data-ttu-id="33e00-126">application/json</span><span class="sxs-lookup"><span data-stu-id="33e00-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33e00-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33e00-127">Request body</span></span>
<span data-ttu-id="33e00-128">No corpo da solicitação, forneça uma representação JSON do objeto [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="33e00-128">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="33e00-129">A tabela a seguir mostra as propriedades obrigatórias ao criar o [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="33e00-129">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="33e00-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33e00-130">Property</span></span>|<span data-ttu-id="33e00-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="33e00-131">Type</span></span>|<span data-ttu-id="33e00-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="33e00-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33e00-133">id</span><span class="sxs-lookup"><span data-stu-id="33e00-133">id</span></span>|<span data-ttu-id="33e00-134">String</span><span class="sxs-lookup"><span data-stu-id="33e00-134">String</span></span>|<span data-ttu-id="33e00-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="33e00-135">Key of the entity.</span></span> <span data-ttu-id="33e00-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="33e00-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33e00-137">displayName</span><span class="sxs-lookup"><span data-stu-id="33e00-137">displayName</span></span>|<span data-ttu-id="33e00-138">String</span><span class="sxs-lookup"><span data-stu-id="33e00-138">String</span></span>|<span data-ttu-id="33e00-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="33e00-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="33e00-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="33e00-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33e00-141">description</span><span class="sxs-lookup"><span data-stu-id="33e00-141">description</span></span>|<span data-ttu-id="33e00-142">String</span><span class="sxs-lookup"><span data-stu-id="33e00-142">String</span></span>|<span data-ttu-id="33e00-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="33e00-143">The description of the app.</span></span> <span data-ttu-id="33e00-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="33e00-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33e00-145">publicador</span><span class="sxs-lookup"><span data-stu-id="33e00-145">publisher</span></span>|<span data-ttu-id="33e00-146">String</span><span class="sxs-lookup"><span data-stu-id="33e00-146">String</span></span>|<span data-ttu-id="33e00-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="33e00-147">The publisher of the app.</span></span> <span data-ttu-id="33e00-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="33e00-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33e00-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="33e00-149">largeIcon</span></span>|[<span data-ttu-id="33e00-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="33e00-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="33e00-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="33e00-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="33e00-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="33e00-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33e00-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="33e00-153">createdDateTime</span></span>|<span data-ttu-id="33e00-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33e00-154">DateTimeOffset</span></span>|<span data-ttu-id="33e00-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="33e00-155">The date and time the app was created.</span></span> <span data-ttu-id="33e00-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="33e00-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33e00-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33e00-157">lastModifiedDateTime</span></span>|<span data-ttu-id="33e00-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33e00-158">DateTimeOffset</span></span>|<span data-ttu-id="33e00-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="33e00-159">The date and time the app was last modified.</span></span> <span data-ttu-id="33e00-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="33e00-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33e00-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="33e00-161">isFeatured</span></span>|<span data-ttu-id="33e00-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="33e00-162">Boolean</span></span>|<span data-ttu-id="33e00-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="33e00-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33e00-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="33e00-164">privacyInformationUrl</span></span>|<span data-ttu-id="33e00-165">String</span><span class="sxs-lookup"><span data-stu-id="33e00-165">String</span></span>|<span data-ttu-id="33e00-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="33e00-166">The privacy statement Url.</span></span> <span data-ttu-id="33e00-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="33e00-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33e00-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="33e00-168">informationUrl</span></span>|<span data-ttu-id="33e00-169">String</span><span class="sxs-lookup"><span data-stu-id="33e00-169">String</span></span>|<span data-ttu-id="33e00-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="33e00-170">The more information Url.</span></span> <span data-ttu-id="33e00-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="33e00-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33e00-172">owner</span><span class="sxs-lookup"><span data-stu-id="33e00-172">owner</span></span>|<span data-ttu-id="33e00-173">String</span><span class="sxs-lookup"><span data-stu-id="33e00-173">String</span></span>|<span data-ttu-id="33e00-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="33e00-174">The owner of the app.</span></span> <span data-ttu-id="33e00-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="33e00-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33e00-176">developer</span><span class="sxs-lookup"><span data-stu-id="33e00-176">developer</span></span>|<span data-ttu-id="33e00-177">String</span><span class="sxs-lookup"><span data-stu-id="33e00-177">String</span></span>|<span data-ttu-id="33e00-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="33e00-178">The developer of the app.</span></span> <span data-ttu-id="33e00-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="33e00-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33e00-180">notes</span><span class="sxs-lookup"><span data-stu-id="33e00-180">notes</span></span>|<span data-ttu-id="33e00-181">String</span><span class="sxs-lookup"><span data-stu-id="33e00-181">String</span></span>|<span data-ttu-id="33e00-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="33e00-182">Notes for the app.</span></span> <span data-ttu-id="33e00-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="33e00-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33e00-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="33e00-184">uploadState</span></span>|<span data-ttu-id="33e00-185">Int32</span><span class="sxs-lookup"><span data-stu-id="33e00-185">Int32</span></span>|<span data-ttu-id="33e00-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="33e00-186">The upload state.</span></span> <span data-ttu-id="33e00-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="33e00-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="33e00-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="33e00-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33e00-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="33e00-189">publishingState</span></span>|[<span data-ttu-id="33e00-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="33e00-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="33e00-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="33e00-191">The publishing state for the app.</span></span> <span data-ttu-id="33e00-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="33e00-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="33e00-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="33e00-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="33e00-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="33e00-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="33e00-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="33e00-195">isAssigned</span></span>|<span data-ttu-id="33e00-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="33e00-196">Boolean</span></span>|<span data-ttu-id="33e00-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="33e00-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="33e00-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="33e00-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33e00-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="33e00-199">roleScopeTagIds</span></span>|<span data-ttu-id="33e00-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="33e00-200">String collection</span></span>|<span data-ttu-id="33e00-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="33e00-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="33e00-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="33e00-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33e00-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="33e00-203">dependentAppCount</span></span>|<span data-ttu-id="33e00-204">Int32</span><span class="sxs-lookup"><span data-stu-id="33e00-204">Int32</span></span>|<span data-ttu-id="33e00-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="33e00-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="33e00-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="33e00-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33e00-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="33e00-207">supersedingAppCount</span></span>|<span data-ttu-id="33e00-208">Int32</span><span class="sxs-lookup"><span data-stu-id="33e00-208">Int32</span></span>|<span data-ttu-id="33e00-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="33e00-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="33e00-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="33e00-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33e00-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="33e00-211">supersededAppCount</span></span>|<span data-ttu-id="33e00-212">Int32</span><span class="sxs-lookup"><span data-stu-id="33e00-212">Int32</span></span>|<span data-ttu-id="33e00-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="33e00-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="33e00-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="33e00-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="33e00-215">appUrl</span><span class="sxs-lookup"><span data-stu-id="33e00-215">appUrl</span></span>|<span data-ttu-id="33e00-216">String</span><span class="sxs-lookup"><span data-stu-id="33e00-216">String</span></span>|<span data-ttu-id="33e00-217">A URL do aplicativo Web.</span><span class="sxs-lookup"><span data-stu-id="33e00-217">The web app URL.</span></span>|
|<span data-ttu-id="33e00-218">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="33e00-218">useManagedBrowser</span></span>|<span data-ttu-id="33e00-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="33e00-219">Boolean</span></span>|<span data-ttu-id="33e00-220">Se o navegador gerenciado deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="33e00-220">Whether or not to use managed browser.</span></span> <span data-ttu-id="33e00-221">Essa propriedade só é aplicável ao Android e ao IOS.</span><span class="sxs-lookup"><span data-stu-id="33e00-221">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="33e00-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="33e00-222">Response</span></span>
<span data-ttu-id="33e00-223">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [webApp](../resources/intune-apps-webapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33e00-223">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33e00-224">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33e00-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="33e00-225">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33e00-225">Request</span></span>
<span data-ttu-id="33e00-226">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33e00-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="33e00-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="33e00-227">Response</span></span>
<span data-ttu-id="33e00-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33e00-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





