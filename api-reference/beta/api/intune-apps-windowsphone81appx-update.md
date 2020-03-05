---
title: Atualizar windowsPhone81AppX
description: Atualiza as propriedades de um objeto windowsPhone81AppX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3259c6686b65793583fe4c9fe17f6af7387901be
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444760"
---
# <a name="update-windowsphone81appx"></a><span data-ttu-id="1ed69-103">Atualizar windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="1ed69-103">Update windowsPhone81AppX</span></span>

<span data-ttu-id="1ed69-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1ed69-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ed69-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1ed69-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ed69-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1ed69-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ed69-107">Atualiza as propriedades de um objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="1ed69-107">Update the properties of a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ed69-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1ed69-108">Prerequisites</span></span>
<span data-ttu-id="1ed69-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ed69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ed69-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ed69-111">Permission type</span></span>|<span data-ttu-id="1ed69-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1ed69-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ed69-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ed69-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ed69-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ed69-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1ed69-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ed69-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ed69-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ed69-116">Not supported.</span></span>|
|<span data-ttu-id="1ed69-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ed69-117">Application</span></span>|<span data-ttu-id="1ed69-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ed69-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ed69-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ed69-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="1ed69-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ed69-120">Request headers</span></span>
|<span data-ttu-id="1ed69-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1ed69-121">Header</span></span>|<span data-ttu-id="1ed69-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1ed69-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ed69-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ed69-123">Authorization</span></span>|<span data-ttu-id="1ed69-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ed69-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ed69-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1ed69-125">Accept</span></span>|<span data-ttu-id="1ed69-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1ed69-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ed69-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ed69-127">Request body</span></span>
<span data-ttu-id="1ed69-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="1ed69-128">In the request body, supply a JSON representation for the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

<span data-ttu-id="1ed69-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="1ed69-129">The following table shows the properties that are required when you create the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span>

|<span data-ttu-id="1ed69-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ed69-130">Property</span></span>|<span data-ttu-id="1ed69-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ed69-131">Type</span></span>|<span data-ttu-id="1ed69-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ed69-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ed69-133">id</span><span class="sxs-lookup"><span data-stu-id="1ed69-133">id</span></span>|<span data-ttu-id="1ed69-134">String</span><span class="sxs-lookup"><span data-stu-id="1ed69-134">String</span></span>|<span data-ttu-id="1ed69-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1ed69-135">Key of the entity.</span></span> <span data-ttu-id="1ed69-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ed69-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ed69-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1ed69-137">displayName</span></span>|<span data-ttu-id="1ed69-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ed69-138">String</span></span>|<span data-ttu-id="1ed69-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="1ed69-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1ed69-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ed69-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ed69-141">description</span><span class="sxs-lookup"><span data-stu-id="1ed69-141">description</span></span>|<span data-ttu-id="1ed69-142">String</span><span class="sxs-lookup"><span data-stu-id="1ed69-142">String</span></span>|<span data-ttu-id="1ed69-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1ed69-143">The description of the app.</span></span> <span data-ttu-id="1ed69-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ed69-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ed69-145">publicador</span><span class="sxs-lookup"><span data-stu-id="1ed69-145">publisher</span></span>|<span data-ttu-id="1ed69-146">String</span><span class="sxs-lookup"><span data-stu-id="1ed69-146">String</span></span>|<span data-ttu-id="1ed69-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1ed69-147">The publisher of the app.</span></span> <span data-ttu-id="1ed69-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ed69-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ed69-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1ed69-149">largeIcon</span></span>|[<span data-ttu-id="1ed69-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1ed69-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1ed69-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="1ed69-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1ed69-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ed69-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ed69-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ed69-153">createdDateTime</span></span>|<span data-ttu-id="1ed69-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ed69-154">DateTimeOffset</span></span>|<span data-ttu-id="1ed69-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1ed69-155">The date and time the app was created.</span></span> <span data-ttu-id="1ed69-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ed69-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ed69-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ed69-157">lastModifiedDateTime</span></span>|<span data-ttu-id="1ed69-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ed69-158">DateTimeOffset</span></span>|<span data-ttu-id="1ed69-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="1ed69-159">The date and time the app was last modified.</span></span> <span data-ttu-id="1ed69-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ed69-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ed69-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1ed69-161">isFeatured</span></span>|<span data-ttu-id="1ed69-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ed69-162">Boolean</span></span>|<span data-ttu-id="1ed69-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ed69-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ed69-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1ed69-164">privacyInformationUrl</span></span>|<span data-ttu-id="1ed69-165">String</span><span class="sxs-lookup"><span data-stu-id="1ed69-165">String</span></span>|<span data-ttu-id="1ed69-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="1ed69-166">The privacy statement Url.</span></span> <span data-ttu-id="1ed69-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ed69-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ed69-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1ed69-168">informationUrl</span></span>|<span data-ttu-id="1ed69-169">String</span><span class="sxs-lookup"><span data-stu-id="1ed69-169">String</span></span>|<span data-ttu-id="1ed69-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="1ed69-170">The more information Url.</span></span> <span data-ttu-id="1ed69-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ed69-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ed69-172">owner</span><span class="sxs-lookup"><span data-stu-id="1ed69-172">owner</span></span>|<span data-ttu-id="1ed69-173">String</span><span class="sxs-lookup"><span data-stu-id="1ed69-173">String</span></span>|<span data-ttu-id="1ed69-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="1ed69-174">The owner of the app.</span></span> <span data-ttu-id="1ed69-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ed69-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ed69-176">developer</span><span class="sxs-lookup"><span data-stu-id="1ed69-176">developer</span></span>|<span data-ttu-id="1ed69-177">String</span><span class="sxs-lookup"><span data-stu-id="1ed69-177">String</span></span>|<span data-ttu-id="1ed69-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1ed69-178">The developer of the app.</span></span> <span data-ttu-id="1ed69-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ed69-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ed69-180">notes</span><span class="sxs-lookup"><span data-stu-id="1ed69-180">notes</span></span>|<span data-ttu-id="1ed69-181">String</span><span class="sxs-lookup"><span data-stu-id="1ed69-181">String</span></span>|<span data-ttu-id="1ed69-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1ed69-182">Notes for the app.</span></span> <span data-ttu-id="1ed69-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ed69-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ed69-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="1ed69-184">uploadState</span></span>|<span data-ttu-id="1ed69-185">Int32</span><span class="sxs-lookup"><span data-stu-id="1ed69-185">Int32</span></span>|<span data-ttu-id="1ed69-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="1ed69-186">The upload state.</span></span> <span data-ttu-id="1ed69-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ed69-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ed69-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="1ed69-188">publishingState</span></span>|[<span data-ttu-id="1ed69-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1ed69-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1ed69-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1ed69-190">The publishing state for the app.</span></span> <span data-ttu-id="1ed69-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="1ed69-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1ed69-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1ed69-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="1ed69-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="1ed69-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1ed69-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1ed69-194">isAssigned</span></span>|<span data-ttu-id="1ed69-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ed69-195">Boolean</span></span>|<span data-ttu-id="1ed69-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="1ed69-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="1ed69-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ed69-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ed69-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1ed69-198">roleScopeTagIds</span></span>|<span data-ttu-id="1ed69-199">String collection</span><span class="sxs-lookup"><span data-stu-id="1ed69-199">String collection</span></span>|<span data-ttu-id="1ed69-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="1ed69-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="1ed69-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ed69-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ed69-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="1ed69-202">dependentAppCount</span></span>|<span data-ttu-id="1ed69-203">Int32</span><span class="sxs-lookup"><span data-stu-id="1ed69-203">Int32</span></span>|<span data-ttu-id="1ed69-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="1ed69-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="1ed69-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ed69-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1ed69-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="1ed69-206">committedContentVersion</span></span>|<span data-ttu-id="1ed69-207">String</span><span class="sxs-lookup"><span data-stu-id="1ed69-207">String</span></span>|<span data-ttu-id="1ed69-208">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="1ed69-208">The internal committed content version.</span></span> <span data-ttu-id="1ed69-209">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ed69-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1ed69-210">fileName</span><span class="sxs-lookup"><span data-stu-id="1ed69-210">fileName</span></span>|<span data-ttu-id="1ed69-211">String</span><span class="sxs-lookup"><span data-stu-id="1ed69-211">String</span></span>|<span data-ttu-id="1ed69-212">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="1ed69-212">The name of the main Lob application file.</span></span> <span data-ttu-id="1ed69-213">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ed69-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1ed69-214">size</span><span class="sxs-lookup"><span data-stu-id="1ed69-214">size</span></span>|<span data-ttu-id="1ed69-215">Int64</span><span class="sxs-lookup"><span data-stu-id="1ed69-215">Int64</span></span>|<span data-ttu-id="1ed69-216">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="1ed69-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="1ed69-217">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ed69-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1ed69-218">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="1ed69-218">applicableArchitectures</span></span>|[<span data-ttu-id="1ed69-219">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="1ed69-219">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="1ed69-220">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="1ed69-220">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="1ed69-221">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="1ed69-221">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="1ed69-222">identityName</span><span class="sxs-lookup"><span data-stu-id="1ed69-222">identityName</span></span>|<span data-ttu-id="1ed69-223">String</span><span class="sxs-lookup"><span data-stu-id="1ed69-223">String</span></span>|<span data-ttu-id="1ed69-224">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="1ed69-224">The Identity Name.</span></span>|
|<span data-ttu-id="1ed69-225">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="1ed69-225">identityPublisherHash</span></span>|<span data-ttu-id="1ed69-226">String</span><span class="sxs-lookup"><span data-stu-id="1ed69-226">String</span></span>|<span data-ttu-id="1ed69-227">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="1ed69-227">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="1ed69-228">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="1ed69-228">identityResourceIdentifier</span></span>|<span data-ttu-id="1ed69-229">String</span><span class="sxs-lookup"><span data-stu-id="1ed69-229">String</span></span>|<span data-ttu-id="1ed69-230">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="1ed69-230">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="1ed69-231">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1ed69-231">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1ed69-232">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1ed69-232">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="1ed69-233">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="1ed69-233">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="1ed69-234">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="1ed69-234">phoneProductIdentifier</span></span>|<span data-ttu-id="1ed69-235">String</span><span class="sxs-lookup"><span data-stu-id="1ed69-235">String</span></span>|<span data-ttu-id="1ed69-236">O identificador do produto de telefone.</span><span class="sxs-lookup"><span data-stu-id="1ed69-236">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="1ed69-237">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="1ed69-237">phonePublisherId</span></span>|<span data-ttu-id="1ed69-238">String</span><span class="sxs-lookup"><span data-stu-id="1ed69-238">String</span></span>|<span data-ttu-id="1ed69-239">A ID do editor do telefone.</span><span class="sxs-lookup"><span data-stu-id="1ed69-239">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="1ed69-240">identityVersion</span><span class="sxs-lookup"><span data-stu-id="1ed69-240">identityVersion</span></span>|<span data-ttu-id="1ed69-241">String</span><span class="sxs-lookup"><span data-stu-id="1ed69-241">String</span></span>|<span data-ttu-id="1ed69-242">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="1ed69-242">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="1ed69-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ed69-243">Response</span></span>
<span data-ttu-id="1ed69-244">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ed69-244">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ed69-245">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ed69-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ed69-246">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ed69-246">Request</span></span>
<span data-ttu-id="1ed69-247">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ed69-247">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1513

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
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
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="1ed69-248">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ed69-248">Response</span></span>
<span data-ttu-id="1ed69-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1ed69-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1685

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
  "id": "4ff27f80-7f80-4ff2-807f-f24f807ff24f",
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
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```





