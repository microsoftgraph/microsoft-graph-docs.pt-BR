---
title: Atualizar windowsUniversalAppX
description: Atualiza as propriedades de um objeto windowsUniversalAppX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3a49b42e050b2dbc9229b71a13dede3a82f8a529
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35959646"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="e263c-103">Atualizar windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="e263c-103">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="e263c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e263c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e263c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e263c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e263c-106">Atualiza as propriedades de um objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="e263c-106">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e263c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e263c-107">Prerequisites</span></span>
<span data-ttu-id="e263c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e263c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e263c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e263c-110">Permission type</span></span>|<span data-ttu-id="e263c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e263c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e263c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e263c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e263c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e263c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e263c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e263c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e263c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e263c-115">Not supported.</span></span>|
|<span data-ttu-id="e263c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e263c-116">Application</span></span>|<span data-ttu-id="e263c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e263c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e263c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e263c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="e263c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e263c-119">Request headers</span></span>
|<span data-ttu-id="e263c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e263c-120">Header</span></span>|<span data-ttu-id="e263c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e263c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e263c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e263c-122">Authorization</span></span>|<span data-ttu-id="e263c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e263c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e263c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e263c-124">Accept</span></span>|<span data-ttu-id="e263c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e263c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e263c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e263c-126">Request body</span></span>
<span data-ttu-id="e263c-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="e263c-127">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="e263c-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="e263c-128">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="e263c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e263c-129">Property</span></span>|<span data-ttu-id="e263c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e263c-130">Type</span></span>|<span data-ttu-id="e263c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e263c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e263c-132">id</span><span class="sxs-lookup"><span data-stu-id="e263c-132">id</span></span>|<span data-ttu-id="e263c-133">String</span><span class="sxs-lookup"><span data-stu-id="e263c-133">String</span></span>|<span data-ttu-id="e263c-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e263c-134">Key of the entity.</span></span> <span data-ttu-id="e263c-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e263c-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e263c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e263c-136">displayName</span></span>|<span data-ttu-id="e263c-137">String</span><span class="sxs-lookup"><span data-stu-id="e263c-137">String</span></span>|<span data-ttu-id="e263c-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="e263c-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e263c-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e263c-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e263c-140">descrição</span><span class="sxs-lookup"><span data-stu-id="e263c-140">description</span></span>|<span data-ttu-id="e263c-141">String</span><span class="sxs-lookup"><span data-stu-id="e263c-141">String</span></span>|<span data-ttu-id="e263c-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e263c-142">The description of the app.</span></span> <span data-ttu-id="e263c-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e263c-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e263c-144">publicador</span><span class="sxs-lookup"><span data-stu-id="e263c-144">publisher</span></span>|<span data-ttu-id="e263c-145">String</span><span class="sxs-lookup"><span data-stu-id="e263c-145">String</span></span>|<span data-ttu-id="e263c-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e263c-146">The publisher of the app.</span></span> <span data-ttu-id="e263c-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e263c-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e263c-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e263c-148">largeIcon</span></span>|[<span data-ttu-id="e263c-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e263c-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e263c-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="e263c-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e263c-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e263c-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e263c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e263c-152">createdDateTime</span></span>|<span data-ttu-id="e263c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e263c-153">DateTimeOffset</span></span>|<span data-ttu-id="e263c-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e263c-154">The date and time the app was created.</span></span> <span data-ttu-id="e263c-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e263c-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e263c-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e263c-156">lastModifiedDateTime</span></span>|<span data-ttu-id="e263c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e263c-157">DateTimeOffset</span></span>|<span data-ttu-id="e263c-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e263c-158">The date and time the app was last modified.</span></span> <span data-ttu-id="e263c-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e263c-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e263c-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e263c-160">isFeatured</span></span>|<span data-ttu-id="e263c-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="e263c-161">Boolean</span></span>|<span data-ttu-id="e263c-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e263c-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e263c-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e263c-163">privacyInformationUrl</span></span>|<span data-ttu-id="e263c-164">String</span><span class="sxs-lookup"><span data-stu-id="e263c-164">String</span></span>|<span data-ttu-id="e263c-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="e263c-165">The privacy statement Url.</span></span> <span data-ttu-id="e263c-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e263c-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e263c-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e263c-167">informationUrl</span></span>|<span data-ttu-id="e263c-168">String</span><span class="sxs-lookup"><span data-stu-id="e263c-168">String</span></span>|<span data-ttu-id="e263c-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="e263c-169">The more information Url.</span></span> <span data-ttu-id="e263c-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e263c-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e263c-171">owner</span><span class="sxs-lookup"><span data-stu-id="e263c-171">owner</span></span>|<span data-ttu-id="e263c-172">String</span><span class="sxs-lookup"><span data-stu-id="e263c-172">String</span></span>|<span data-ttu-id="e263c-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e263c-173">The owner of the app.</span></span> <span data-ttu-id="e263c-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e263c-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e263c-175">developer</span><span class="sxs-lookup"><span data-stu-id="e263c-175">developer</span></span>|<span data-ttu-id="e263c-176">String</span><span class="sxs-lookup"><span data-stu-id="e263c-176">String</span></span>|<span data-ttu-id="e263c-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e263c-177">The developer of the app.</span></span> <span data-ttu-id="e263c-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e263c-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e263c-179">notes</span><span class="sxs-lookup"><span data-stu-id="e263c-179">notes</span></span>|<span data-ttu-id="e263c-180">String</span><span class="sxs-lookup"><span data-stu-id="e263c-180">String</span></span>|<span data-ttu-id="e263c-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e263c-181">Notes for the app.</span></span> <span data-ttu-id="e263c-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e263c-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e263c-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="e263c-183">uploadState</span></span>|<span data-ttu-id="e263c-184">Int32</span><span class="sxs-lookup"><span data-stu-id="e263c-184">Int32</span></span>|<span data-ttu-id="e263c-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="e263c-185">The upload state.</span></span> <span data-ttu-id="e263c-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e263c-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e263c-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="e263c-187">publishingState</span></span>|[<span data-ttu-id="e263c-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e263c-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e263c-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e263c-189">The publishing state for the app.</span></span> <span data-ttu-id="e263c-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="e263c-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e263c-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e263c-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e263c-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e263c-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e263c-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e263c-193">isAssigned</span></span>|<span data-ttu-id="e263c-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="e263c-194">Boolean</span></span>|<span data-ttu-id="e263c-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="e263c-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e263c-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e263c-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e263c-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e263c-197">roleScopeTagIds</span></span>|<span data-ttu-id="e263c-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e263c-198">String collection</span></span>|<span data-ttu-id="e263c-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="e263c-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e263c-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e263c-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e263c-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="e263c-201">dependentAppCount</span></span>|<span data-ttu-id="e263c-202">Int32</span><span class="sxs-lookup"><span data-stu-id="e263c-202">Int32</span></span>|<span data-ttu-id="e263c-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="e263c-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="e263c-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e263c-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e263c-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e263c-205">committedContentVersion</span></span>|<span data-ttu-id="e263c-206">String</span><span class="sxs-lookup"><span data-stu-id="e263c-206">String</span></span>|<span data-ttu-id="e263c-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="e263c-207">The internal committed content version.</span></span> <span data-ttu-id="e263c-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e263c-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e263c-209">fileName</span><span class="sxs-lookup"><span data-stu-id="e263c-209">fileName</span></span>|<span data-ttu-id="e263c-210">String</span><span class="sxs-lookup"><span data-stu-id="e263c-210">String</span></span>|<span data-ttu-id="e263c-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="e263c-211">The name of the main Lob application file.</span></span> <span data-ttu-id="e263c-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e263c-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e263c-213">size</span><span class="sxs-lookup"><span data-stu-id="e263c-213">size</span></span>|<span data-ttu-id="e263c-214">Int64</span><span class="sxs-lookup"><span data-stu-id="e263c-214">Int64</span></span>|<span data-ttu-id="e263c-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="e263c-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="e263c-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e263c-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e263c-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="e263c-217">applicableArchitectures</span></span>|[<span data-ttu-id="e263c-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="e263c-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="e263c-219">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="e263c-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="e263c-220">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="e263c-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="e263c-221">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="e263c-221">applicableDeviceTypes</span></span>|[<span data-ttu-id="e263c-222">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="e263c-222">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="e263c-223">Os tipos de dispositivos Windows nos quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="e263c-223">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="e263c-224">Os valores possíveis são: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="e263c-224">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="e263c-225">identityName</span><span class="sxs-lookup"><span data-stu-id="e263c-225">identityName</span></span>|<span data-ttu-id="e263c-226">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e263c-226">String</span></span>|<span data-ttu-id="e263c-227">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="e263c-227">The Identity Name.</span></span>|
|<span data-ttu-id="e263c-228">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="e263c-228">identityPublisherHash</span></span>|<span data-ttu-id="e263c-229">String</span><span class="sxs-lookup"><span data-stu-id="e263c-229">String</span></span>|<span data-ttu-id="e263c-230">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="e263c-230">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="e263c-231">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="e263c-231">identityResourceIdentifier</span></span>|<span data-ttu-id="e263c-232">String</span><span class="sxs-lookup"><span data-stu-id="e263c-232">String</span></span>|<span data-ttu-id="e263c-233">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="e263c-233">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="e263c-234">isBundle</span><span class="sxs-lookup"><span data-stu-id="e263c-234">isBundle</span></span>|<span data-ttu-id="e263c-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="e263c-235">Boolean</span></span>|<span data-ttu-id="e263c-236">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="e263c-236">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="e263c-237">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e263c-237">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e263c-238">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e263c-238">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="e263c-239">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="e263c-239">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e263c-240">identityVersion</span><span class="sxs-lookup"><span data-stu-id="e263c-240">identityVersion</span></span>|<span data-ttu-id="e263c-241">String</span><span class="sxs-lookup"><span data-stu-id="e263c-241">String</span></span>|<span data-ttu-id="e263c-242">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="e263c-242">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="e263c-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="e263c-243">Response</span></span>
<span data-ttu-id="e263c-244">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e263c-244">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e263c-245">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e263c-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="e263c-246">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e263c-246">Request</span></span>
<span data-ttu-id="e263c-247">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e263c-247">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1461

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "applicableDeviceTypes": "desktop",
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

### <a name="response"></a><span data-ttu-id="e263c-248">Resposta</span><span class="sxs-lookup"><span data-stu-id="e263c-248">Response</span></span>
<span data-ttu-id="e263c-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e263c-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1633

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "applicableDeviceTypes": "desktop",
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





