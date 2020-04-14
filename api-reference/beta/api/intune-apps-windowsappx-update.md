---
title: Atualizar windowsAppX
description: Atualiza as propriedades de um objeto windowsAppX.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 539e4129757a00e2083da9c50d79d7a6d736de87
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43393690"
---
# <a name="update-windowsappx"></a><span data-ttu-id="6dc62-103">Atualizar windowsAppX</span><span class="sxs-lookup"><span data-stu-id="6dc62-103">Update windowsAppX</span></span>

<span data-ttu-id="6dc62-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6dc62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6dc62-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6dc62-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6dc62-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6dc62-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dc62-107">Atualiza as propriedades de um objeto [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="6dc62-107">Update the properties of a [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6dc62-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6dc62-108">Prerequisites</span></span>
<span data-ttu-id="6dc62-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dc62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dc62-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6dc62-111">Permission type</span></span>|<span data-ttu-id="6dc62-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6dc62-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dc62-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6dc62-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6dc62-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dc62-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6dc62-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6dc62-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dc62-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6dc62-116">Not supported.</span></span>|
|<span data-ttu-id="6dc62-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6dc62-117">Application</span></span>|<span data-ttu-id="6dc62-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dc62-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dc62-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6dc62-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="6dc62-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6dc62-120">Request headers</span></span>
|<span data-ttu-id="6dc62-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6dc62-121">Header</span></span>|<span data-ttu-id="6dc62-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6dc62-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6dc62-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6dc62-123">Authorization</span></span>|<span data-ttu-id="6dc62-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6dc62-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6dc62-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6dc62-125">Accept</span></span>|<span data-ttu-id="6dc62-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6dc62-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dc62-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6dc62-127">Request body</span></span>
<span data-ttu-id="6dc62-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="6dc62-128">In the request body, supply a JSON representation for the [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

<span data-ttu-id="6dc62-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsAppX](../resources/intune-apps-windowsappx.md).</span><span class="sxs-lookup"><span data-stu-id="6dc62-129">The following table shows the properties that are required when you create the [windowsAppX](../resources/intune-apps-windowsappx.md).</span></span>

|<span data-ttu-id="6dc62-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6dc62-130">Property</span></span>|<span data-ttu-id="6dc62-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6dc62-131">Type</span></span>|<span data-ttu-id="6dc62-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dc62-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dc62-133">id</span><span class="sxs-lookup"><span data-stu-id="6dc62-133">id</span></span>|<span data-ttu-id="6dc62-134">String</span><span class="sxs-lookup"><span data-stu-id="6dc62-134">String</span></span>|<span data-ttu-id="6dc62-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6dc62-135">Key of the entity.</span></span> <span data-ttu-id="6dc62-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6dc62-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6dc62-137">displayName</span><span class="sxs-lookup"><span data-stu-id="6dc62-137">displayName</span></span>|<span data-ttu-id="6dc62-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6dc62-138">String</span></span>|<span data-ttu-id="6dc62-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="6dc62-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6dc62-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6dc62-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6dc62-141">description</span><span class="sxs-lookup"><span data-stu-id="6dc62-141">description</span></span>|<span data-ttu-id="6dc62-142">String</span><span class="sxs-lookup"><span data-stu-id="6dc62-142">String</span></span>|<span data-ttu-id="6dc62-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6dc62-143">The description of the app.</span></span> <span data-ttu-id="6dc62-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6dc62-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6dc62-145">publicador</span><span class="sxs-lookup"><span data-stu-id="6dc62-145">publisher</span></span>|<span data-ttu-id="6dc62-146">String</span><span class="sxs-lookup"><span data-stu-id="6dc62-146">String</span></span>|<span data-ttu-id="6dc62-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6dc62-147">The publisher of the app.</span></span> <span data-ttu-id="6dc62-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6dc62-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6dc62-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6dc62-149">largeIcon</span></span>|[<span data-ttu-id="6dc62-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6dc62-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6dc62-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="6dc62-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6dc62-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6dc62-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6dc62-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6dc62-153">createdDateTime</span></span>|<span data-ttu-id="6dc62-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6dc62-154">DateTimeOffset</span></span>|<span data-ttu-id="6dc62-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6dc62-155">The date and time the app was created.</span></span> <span data-ttu-id="6dc62-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6dc62-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6dc62-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6dc62-157">lastModifiedDateTime</span></span>|<span data-ttu-id="6dc62-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6dc62-158">DateTimeOffset</span></span>|<span data-ttu-id="6dc62-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6dc62-159">The date and time the app was last modified.</span></span> <span data-ttu-id="6dc62-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6dc62-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6dc62-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6dc62-161">isFeatured</span></span>|<span data-ttu-id="6dc62-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="6dc62-162">Boolean</span></span>|<span data-ttu-id="6dc62-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6dc62-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6dc62-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6dc62-164">privacyInformationUrl</span></span>|<span data-ttu-id="6dc62-165">String</span><span class="sxs-lookup"><span data-stu-id="6dc62-165">String</span></span>|<span data-ttu-id="6dc62-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="6dc62-166">The privacy statement Url.</span></span> <span data-ttu-id="6dc62-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6dc62-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6dc62-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6dc62-168">informationUrl</span></span>|<span data-ttu-id="6dc62-169">String</span><span class="sxs-lookup"><span data-stu-id="6dc62-169">String</span></span>|<span data-ttu-id="6dc62-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="6dc62-170">The more information Url.</span></span> <span data-ttu-id="6dc62-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6dc62-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6dc62-172">owner</span><span class="sxs-lookup"><span data-stu-id="6dc62-172">owner</span></span>|<span data-ttu-id="6dc62-173">String</span><span class="sxs-lookup"><span data-stu-id="6dc62-173">String</span></span>|<span data-ttu-id="6dc62-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="6dc62-174">The owner of the app.</span></span> <span data-ttu-id="6dc62-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6dc62-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6dc62-176">developer</span><span class="sxs-lookup"><span data-stu-id="6dc62-176">developer</span></span>|<span data-ttu-id="6dc62-177">String</span><span class="sxs-lookup"><span data-stu-id="6dc62-177">String</span></span>|<span data-ttu-id="6dc62-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6dc62-178">The developer of the app.</span></span> <span data-ttu-id="6dc62-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6dc62-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6dc62-180">notes</span><span class="sxs-lookup"><span data-stu-id="6dc62-180">notes</span></span>|<span data-ttu-id="6dc62-181">String</span><span class="sxs-lookup"><span data-stu-id="6dc62-181">String</span></span>|<span data-ttu-id="6dc62-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6dc62-182">Notes for the app.</span></span> <span data-ttu-id="6dc62-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6dc62-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6dc62-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="6dc62-184">uploadState</span></span>|<span data-ttu-id="6dc62-185">Int32</span><span class="sxs-lookup"><span data-stu-id="6dc62-185">Int32</span></span>|<span data-ttu-id="6dc62-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="6dc62-186">The upload state.</span></span> <span data-ttu-id="6dc62-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6dc62-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6dc62-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="6dc62-188">publishingState</span></span>|[<span data-ttu-id="6dc62-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="6dc62-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6dc62-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6dc62-190">The publishing state for the app.</span></span> <span data-ttu-id="6dc62-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="6dc62-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6dc62-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6dc62-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="6dc62-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="6dc62-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6dc62-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="6dc62-194">isAssigned</span></span>|<span data-ttu-id="6dc62-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="6dc62-195">Boolean</span></span>|<span data-ttu-id="6dc62-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="6dc62-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="6dc62-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6dc62-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6dc62-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6dc62-198">roleScopeTagIds</span></span>|<span data-ttu-id="6dc62-199">Coleção String</span><span class="sxs-lookup"><span data-stu-id="6dc62-199">String collection</span></span>|<span data-ttu-id="6dc62-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="6dc62-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="6dc62-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6dc62-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6dc62-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="6dc62-202">dependentAppCount</span></span>|<span data-ttu-id="6dc62-203">Int32</span><span class="sxs-lookup"><span data-stu-id="6dc62-203">Int32</span></span>|<span data-ttu-id="6dc62-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="6dc62-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="6dc62-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6dc62-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6dc62-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="6dc62-206">committedContentVersion</span></span>|<span data-ttu-id="6dc62-207">String</span><span class="sxs-lookup"><span data-stu-id="6dc62-207">String</span></span>|<span data-ttu-id="6dc62-208">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="6dc62-208">The internal committed content version.</span></span> <span data-ttu-id="6dc62-209">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="6dc62-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="6dc62-210">fileName</span><span class="sxs-lookup"><span data-stu-id="6dc62-210">fileName</span></span>|<span data-ttu-id="6dc62-211">String</span><span class="sxs-lookup"><span data-stu-id="6dc62-211">String</span></span>|<span data-ttu-id="6dc62-212">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="6dc62-212">The name of the main Lob application file.</span></span> <span data-ttu-id="6dc62-213">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="6dc62-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="6dc62-214">size</span><span class="sxs-lookup"><span data-stu-id="6dc62-214">size</span></span>|<span data-ttu-id="6dc62-215">Int64</span><span class="sxs-lookup"><span data-stu-id="6dc62-215">Int64</span></span>|<span data-ttu-id="6dc62-216">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="6dc62-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="6dc62-217">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="6dc62-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="6dc62-218">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="6dc62-218">applicableArchitectures</span></span>|[<span data-ttu-id="6dc62-219">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="6dc62-219">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="6dc62-220">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="6dc62-220">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="6dc62-221">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="6dc62-221">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="6dc62-222">identityName</span><span class="sxs-lookup"><span data-stu-id="6dc62-222">identityName</span></span>|<span data-ttu-id="6dc62-223">String</span><span class="sxs-lookup"><span data-stu-id="6dc62-223">String</span></span>|<span data-ttu-id="6dc62-224">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="6dc62-224">The Identity Name.</span></span>|
|<span data-ttu-id="6dc62-225">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="6dc62-225">identityPublisherHash</span></span>|<span data-ttu-id="6dc62-226">String</span><span class="sxs-lookup"><span data-stu-id="6dc62-226">String</span></span>|<span data-ttu-id="6dc62-227">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="6dc62-227">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="6dc62-228">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="6dc62-228">identityResourceIdentifier</span></span>|<span data-ttu-id="6dc62-229">String</span><span class="sxs-lookup"><span data-stu-id="6dc62-229">String</span></span>|<span data-ttu-id="6dc62-230">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="6dc62-230">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="6dc62-231">isBundle</span><span class="sxs-lookup"><span data-stu-id="6dc62-231">isBundle</span></span>|<span data-ttu-id="6dc62-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="6dc62-232">Boolean</span></span>|<span data-ttu-id="6dc62-233">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="6dc62-233">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="6dc62-234">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6dc62-234">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="6dc62-235">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6dc62-235">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="6dc62-236">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="6dc62-236">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="6dc62-237">identityVersion</span><span class="sxs-lookup"><span data-stu-id="6dc62-237">identityVersion</span></span>|<span data-ttu-id="6dc62-238">String</span><span class="sxs-lookup"><span data-stu-id="6dc62-238">String</span></span>|<span data-ttu-id="6dc62-239">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="6dc62-239">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="6dc62-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dc62-240">Response</span></span>
<span data-ttu-id="6dc62-241">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsAppX](../resources/intune-apps-windowsappx.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6dc62-241">If successful, this method returns a `200 OK` response code and an updated [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dc62-242">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6dc62-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="6dc62-243">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6dc62-243">Request</span></span>
<span data-ttu-id="6dc62-244">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6dc62-244">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1413

{
  "@odata.type": "#microsoft.graph.windowsAppX",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="6dc62-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dc62-245">Response</span></span>
<span data-ttu-id="6dc62-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6dc62-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1585

{
  "@odata.type": "#microsoft.graph.windowsAppX",
  "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "identityVersion": "Identity Version value"
}
```



