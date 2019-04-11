---
title: Atualizar windowsAppX
description: Atualiza as propriedades de um objeto windowsAppX.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3cc1fc2c72cab28d2ed6602673eb13793190d892
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785045"
---
# <a name="update-windowsappx"></a><span data-ttu-id="4973f-103">Atualizar windowsAppX</span><span class="sxs-lookup"><span data-stu-id="4973f-103">Update windowsAppX</span></span>

> <span data-ttu-id="4973f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4973f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4973f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4973f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4973f-106">Atualiza as propriedades de um objeto [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="4973f-106">Update the properties of a [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4973f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4973f-107">Prerequisites</span></span>
<span data-ttu-id="4973f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4973f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4973f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4973f-110">Permission type</span></span>|<span data-ttu-id="4973f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4973f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4973f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4973f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4973f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4973f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4973f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4973f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4973f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4973f-115">Not supported.</span></span>|
|<span data-ttu-id="4973f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4973f-116">Application</span></span>|<span data-ttu-id="4973f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4973f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4973f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4973f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="4973f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4973f-119">Request headers</span></span>
|<span data-ttu-id="4973f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4973f-120">Header</span></span>|<span data-ttu-id="4973f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4973f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4973f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4973f-122">Authorization</span></span>|<span data-ttu-id="4973f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4973f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4973f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4973f-124">Accept</span></span>|<span data-ttu-id="4973f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4973f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4973f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4973f-126">Request body</span></span>
<span data-ttu-id="4973f-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="4973f-127">In the request body, supply a JSON representation for the [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

<span data-ttu-id="4973f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsAppX](../resources/intune-apps-windowsappx.md).</span><span class="sxs-lookup"><span data-stu-id="4973f-128">The following table shows the properties that are required when you create the [windowsAppX](../resources/intune-apps-windowsappx.md).</span></span>

|<span data-ttu-id="4973f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4973f-129">Property</span></span>|<span data-ttu-id="4973f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4973f-130">Type</span></span>|<span data-ttu-id="4973f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4973f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4973f-132">id</span><span class="sxs-lookup"><span data-stu-id="4973f-132">id</span></span>|<span data-ttu-id="4973f-133">String</span><span class="sxs-lookup"><span data-stu-id="4973f-133">String</span></span>|<span data-ttu-id="4973f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4973f-134">Key of the entity.</span></span> <span data-ttu-id="4973f-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4973f-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4973f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4973f-136">displayName</span></span>|<span data-ttu-id="4973f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4973f-137">String</span></span>|<span data-ttu-id="4973f-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="4973f-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4973f-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4973f-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4973f-140">description</span><span class="sxs-lookup"><span data-stu-id="4973f-140">description</span></span>|<span data-ttu-id="4973f-141">String</span><span class="sxs-lookup"><span data-stu-id="4973f-141">String</span></span>|<span data-ttu-id="4973f-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4973f-142">The description of the app.</span></span> <span data-ttu-id="4973f-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4973f-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4973f-144">publicador</span><span class="sxs-lookup"><span data-stu-id="4973f-144">publisher</span></span>|<span data-ttu-id="4973f-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4973f-145">String</span></span>|<span data-ttu-id="4973f-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4973f-146">The publisher of the app.</span></span> <span data-ttu-id="4973f-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4973f-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4973f-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4973f-148">largeIcon</span></span>|[<span data-ttu-id="4973f-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4973f-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4973f-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="4973f-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4973f-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4973f-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4973f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4973f-152">createdDateTime</span></span>|<span data-ttu-id="4973f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4973f-153">DateTimeOffset</span></span>|<span data-ttu-id="4973f-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4973f-154">The date and time the app was created.</span></span> <span data-ttu-id="4973f-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4973f-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4973f-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4973f-156">lastModifiedDateTime</span></span>|<span data-ttu-id="4973f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4973f-157">DateTimeOffset</span></span>|<span data-ttu-id="4973f-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4973f-158">The date and time the app was last modified.</span></span> <span data-ttu-id="4973f-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4973f-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4973f-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4973f-160">isFeatured</span></span>|<span data-ttu-id="4973f-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="4973f-161">Boolean</span></span>|<span data-ttu-id="4973f-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4973f-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4973f-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4973f-163">privacyInformationUrl</span></span>|<span data-ttu-id="4973f-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4973f-164">String</span></span>|<span data-ttu-id="4973f-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="4973f-165">The privacy statement Url.</span></span> <span data-ttu-id="4973f-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4973f-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4973f-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4973f-167">informationUrl</span></span>|<span data-ttu-id="4973f-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4973f-168">String</span></span>|<span data-ttu-id="4973f-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="4973f-169">The more information Url.</span></span> <span data-ttu-id="4973f-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4973f-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4973f-171">owner</span><span class="sxs-lookup"><span data-stu-id="4973f-171">owner</span></span>|<span data-ttu-id="4973f-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4973f-172">String</span></span>|<span data-ttu-id="4973f-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4973f-173">The owner of the app.</span></span> <span data-ttu-id="4973f-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4973f-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4973f-175">developer</span><span class="sxs-lookup"><span data-stu-id="4973f-175">developer</span></span>|<span data-ttu-id="4973f-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4973f-176">String</span></span>|<span data-ttu-id="4973f-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4973f-177">The developer of the app.</span></span> <span data-ttu-id="4973f-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4973f-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4973f-179">notes</span><span class="sxs-lookup"><span data-stu-id="4973f-179">notes</span></span>|<span data-ttu-id="4973f-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4973f-180">String</span></span>|<span data-ttu-id="4973f-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4973f-181">Notes for the app.</span></span> <span data-ttu-id="4973f-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4973f-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4973f-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="4973f-183">uploadState</span></span>|<span data-ttu-id="4973f-184">Int32</span><span class="sxs-lookup"><span data-stu-id="4973f-184">Int32</span></span>|<span data-ttu-id="4973f-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="4973f-185">The upload state.</span></span> <span data-ttu-id="4973f-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4973f-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4973f-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="4973f-187">publishingState</span></span>|[<span data-ttu-id="4973f-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4973f-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4973f-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4973f-189">The publishing state for the app.</span></span> <span data-ttu-id="4973f-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="4973f-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4973f-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4973f-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4973f-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4973f-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4973f-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4973f-193">isAssigned</span></span>|<span data-ttu-id="4973f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4973f-194">Boolean</span></span>|<span data-ttu-id="4973f-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="4973f-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4973f-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4973f-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4973f-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4973f-197">roleScopeTagIds</span></span>|<span data-ttu-id="4973f-198">Coleção String</span><span class="sxs-lookup"><span data-stu-id="4973f-198">String collection</span></span>|<span data-ttu-id="4973f-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="4973f-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4973f-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4973f-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4973f-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="4973f-201">dependentAppCount</span></span>|<span data-ttu-id="4973f-202">Int32</span><span class="sxs-lookup"><span data-stu-id="4973f-202">Int32</span></span>|<span data-ttu-id="4973f-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="4973f-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="4973f-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4973f-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4973f-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="4973f-205">committedContentVersion</span></span>|<span data-ttu-id="4973f-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4973f-206">String</span></span>|<span data-ttu-id="4973f-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="4973f-207">The internal committed content version.</span></span> <span data-ttu-id="4973f-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4973f-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4973f-209">fileName</span><span class="sxs-lookup"><span data-stu-id="4973f-209">fileName</span></span>|<span data-ttu-id="4973f-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4973f-210">String</span></span>|<span data-ttu-id="4973f-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="4973f-211">The name of the main Lob application file.</span></span> <span data-ttu-id="4973f-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4973f-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4973f-213">size</span><span class="sxs-lookup"><span data-stu-id="4973f-213">size</span></span>|<span data-ttu-id="4973f-214">Int64</span><span class="sxs-lookup"><span data-stu-id="4973f-214">Int64</span></span>|<span data-ttu-id="4973f-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="4973f-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="4973f-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4973f-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4973f-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="4973f-217">applicableArchitectures</span></span>|[<span data-ttu-id="4973f-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="4973f-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="4973f-219">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="4973f-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="4973f-220">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="4973f-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="4973f-221">identityName</span><span class="sxs-lookup"><span data-stu-id="4973f-221">identityName</span></span>|<span data-ttu-id="4973f-222">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4973f-222">String</span></span>|<span data-ttu-id="4973f-223">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="4973f-223">The Identity Name.</span></span>|
|<span data-ttu-id="4973f-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="4973f-224">identityPublisherHash</span></span>|<span data-ttu-id="4973f-225">String</span><span class="sxs-lookup"><span data-stu-id="4973f-225">String</span></span>|<span data-ttu-id="4973f-226">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="4973f-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="4973f-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="4973f-227">identityResourceIdentifier</span></span>|<span data-ttu-id="4973f-228">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4973f-228">String</span></span>|<span data-ttu-id="4973f-229">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="4973f-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="4973f-230">isBundle</span><span class="sxs-lookup"><span data-stu-id="4973f-230">isBundle</span></span>|<span data-ttu-id="4973f-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="4973f-231">Boolean</span></span>|<span data-ttu-id="4973f-232">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="4973f-232">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="4973f-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4973f-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4973f-234">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4973f-234">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="4973f-235">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="4973f-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="4973f-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="4973f-236">identityVersion</span></span>|<span data-ttu-id="4973f-237">String</span><span class="sxs-lookup"><span data-stu-id="4973f-237">String</span></span>|<span data-ttu-id="4973f-238">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="4973f-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="4973f-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="4973f-239">Response</span></span>
<span data-ttu-id="4973f-240">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsAppX](../resources/intune-apps-windowsappx.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4973f-240">If successful, this method returns a `200 OK` response code and an updated [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4973f-241">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4973f-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="4973f-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4973f-242">Request</span></span>
<span data-ttu-id="4973f-243">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4973f-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1367

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
    "v10_1803": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="4973f-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="4973f-244">Response</span></span>
<span data-ttu-id="4973f-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4973f-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1539

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
    "v10_1803": true
  },
  "identityVersion": "Identity Version value"
}
```





