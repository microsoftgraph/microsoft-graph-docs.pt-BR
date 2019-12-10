---
title: Atualizar windowsPhone81AppX
description: Atualiza as propriedades de um objeto windowsPhone81AppX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cc367988329a65d0f71e8bc894ed45bab3c11de0
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39933276"
---
# <a name="update-windowsphone81appx"></a><span data-ttu-id="014f4-103">Atualizar windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="014f4-103">Update windowsPhone81AppX</span></span>

> <span data-ttu-id="014f4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="014f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="014f4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="014f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="014f4-106">Atualiza as propriedades de um objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="014f4-106">Update the properties of a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="014f4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="014f4-107">Prerequisites</span></span>
<span data-ttu-id="014f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="014f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="014f4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="014f4-110">Permission type</span></span>|<span data-ttu-id="014f4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="014f4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="014f4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="014f4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="014f4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="014f4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="014f4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="014f4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="014f4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="014f4-115">Not supported.</span></span>|
|<span data-ttu-id="014f4-116">Application</span><span class="sxs-lookup"><span data-stu-id="014f4-116">Application</span></span>|<span data-ttu-id="014f4-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="014f4-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="014f4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="014f4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="014f4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="014f4-119">Request headers</span></span>
|<span data-ttu-id="014f4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="014f4-120">Header</span></span>|<span data-ttu-id="014f4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="014f4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="014f4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="014f4-122">Authorization</span></span>|<span data-ttu-id="014f4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="014f4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="014f4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="014f4-124">Accept</span></span>|<span data-ttu-id="014f4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="014f4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="014f4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="014f4-126">Request body</span></span>
<span data-ttu-id="014f4-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="014f4-127">In the request body, supply a JSON representation for the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

<span data-ttu-id="014f4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="014f4-128">The following table shows the properties that are required when you create the [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span>

|<span data-ttu-id="014f4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="014f4-129">Property</span></span>|<span data-ttu-id="014f4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="014f4-130">Type</span></span>|<span data-ttu-id="014f4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="014f4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="014f4-132">id</span><span class="sxs-lookup"><span data-stu-id="014f4-132">id</span></span>|<span data-ttu-id="014f4-133">String</span><span class="sxs-lookup"><span data-stu-id="014f4-133">String</span></span>|<span data-ttu-id="014f4-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="014f4-134">Key of the entity.</span></span> <span data-ttu-id="014f4-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="014f4-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="014f4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="014f4-136">displayName</span></span>|<span data-ttu-id="014f4-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="014f4-137">String</span></span>|<span data-ttu-id="014f4-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="014f4-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="014f4-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="014f4-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="014f4-140">description</span><span class="sxs-lookup"><span data-stu-id="014f4-140">description</span></span>|<span data-ttu-id="014f4-141">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="014f4-141">String</span></span>|<span data-ttu-id="014f4-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="014f4-142">The description of the app.</span></span> <span data-ttu-id="014f4-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="014f4-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="014f4-144">publicador</span><span class="sxs-lookup"><span data-stu-id="014f4-144">publisher</span></span>|<span data-ttu-id="014f4-145">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="014f4-145">String</span></span>|<span data-ttu-id="014f4-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="014f4-146">The publisher of the app.</span></span> <span data-ttu-id="014f4-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="014f4-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="014f4-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="014f4-148">largeIcon</span></span>|[<span data-ttu-id="014f4-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="014f4-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="014f4-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="014f4-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="014f4-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="014f4-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="014f4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="014f4-152">createdDateTime</span></span>|<span data-ttu-id="014f4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="014f4-153">DateTimeOffset</span></span>|<span data-ttu-id="014f4-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="014f4-154">The date and time the app was created.</span></span> <span data-ttu-id="014f4-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="014f4-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="014f4-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="014f4-156">lastModifiedDateTime</span></span>|<span data-ttu-id="014f4-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="014f4-157">DateTimeOffset</span></span>|<span data-ttu-id="014f4-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="014f4-158">The date and time the app was last modified.</span></span> <span data-ttu-id="014f4-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="014f4-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="014f4-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="014f4-160">isFeatured</span></span>|<span data-ttu-id="014f4-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="014f4-161">Boolean</span></span>|<span data-ttu-id="014f4-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="014f4-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="014f4-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="014f4-163">privacyInformationUrl</span></span>|<span data-ttu-id="014f4-164">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="014f4-164">String</span></span>|<span data-ttu-id="014f4-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="014f4-165">The privacy statement Url.</span></span> <span data-ttu-id="014f4-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="014f4-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="014f4-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="014f4-167">informationUrl</span></span>|<span data-ttu-id="014f4-168">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="014f4-168">String</span></span>|<span data-ttu-id="014f4-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="014f4-169">The more information Url.</span></span> <span data-ttu-id="014f4-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="014f4-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="014f4-171">owner</span><span class="sxs-lookup"><span data-stu-id="014f4-171">owner</span></span>|<span data-ttu-id="014f4-172">String</span><span class="sxs-lookup"><span data-stu-id="014f4-172">String</span></span>|<span data-ttu-id="014f4-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="014f4-173">The owner of the app.</span></span> <span data-ttu-id="014f4-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="014f4-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="014f4-175">developer</span><span class="sxs-lookup"><span data-stu-id="014f4-175">developer</span></span>|<span data-ttu-id="014f4-176">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="014f4-176">String</span></span>|<span data-ttu-id="014f4-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="014f4-177">The developer of the app.</span></span> <span data-ttu-id="014f4-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="014f4-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="014f4-179">notes</span><span class="sxs-lookup"><span data-stu-id="014f4-179">notes</span></span>|<span data-ttu-id="014f4-180">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="014f4-180">String</span></span>|<span data-ttu-id="014f4-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="014f4-181">Notes for the app.</span></span> <span data-ttu-id="014f4-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="014f4-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="014f4-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="014f4-183">uploadState</span></span>|<span data-ttu-id="014f4-184">Int32</span><span class="sxs-lookup"><span data-stu-id="014f4-184">Int32</span></span>|<span data-ttu-id="014f4-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="014f4-185">The upload state.</span></span> <span data-ttu-id="014f4-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="014f4-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="014f4-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="014f4-187">publishingState</span></span>|[<span data-ttu-id="014f4-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="014f4-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="014f4-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="014f4-189">The publishing state for the app.</span></span> <span data-ttu-id="014f4-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="014f4-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="014f4-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="014f4-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="014f4-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="014f4-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="014f4-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="014f4-193">isAssigned</span></span>|<span data-ttu-id="014f4-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="014f4-194">Boolean</span></span>|<span data-ttu-id="014f4-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="014f4-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="014f4-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="014f4-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="014f4-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="014f4-197">roleScopeTagIds</span></span>|<span data-ttu-id="014f4-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="014f4-198">String collection</span></span>|<span data-ttu-id="014f4-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="014f4-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="014f4-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="014f4-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="014f4-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="014f4-201">dependentAppCount</span></span>|<span data-ttu-id="014f4-202">Int32</span><span class="sxs-lookup"><span data-stu-id="014f4-202">Int32</span></span>|<span data-ttu-id="014f4-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="014f4-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="014f4-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="014f4-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="014f4-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="014f4-205">committedContentVersion</span></span>|<span data-ttu-id="014f4-206">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="014f4-206">String</span></span>|<span data-ttu-id="014f4-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="014f4-207">The internal committed content version.</span></span> <span data-ttu-id="014f4-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="014f4-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="014f4-209">fileName</span><span class="sxs-lookup"><span data-stu-id="014f4-209">fileName</span></span>|<span data-ttu-id="014f4-210">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="014f4-210">String</span></span>|<span data-ttu-id="014f4-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="014f4-211">The name of the main Lob application file.</span></span> <span data-ttu-id="014f4-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="014f4-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="014f4-213">size</span><span class="sxs-lookup"><span data-stu-id="014f4-213">size</span></span>|<span data-ttu-id="014f4-214">Int64</span><span class="sxs-lookup"><span data-stu-id="014f4-214">Int64</span></span>|<span data-ttu-id="014f4-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="014f4-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="014f4-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="014f4-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="014f4-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="014f4-217">applicableArchitectures</span></span>|[<span data-ttu-id="014f4-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="014f4-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="014f4-219">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="014f4-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="014f4-220">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="014f4-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="014f4-221">identityName</span><span class="sxs-lookup"><span data-stu-id="014f4-221">identityName</span></span>|<span data-ttu-id="014f4-222">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="014f4-222">String</span></span>|<span data-ttu-id="014f4-223">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="014f4-223">The Identity Name.</span></span>|
|<span data-ttu-id="014f4-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="014f4-224">identityPublisherHash</span></span>|<span data-ttu-id="014f4-225">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="014f4-225">String</span></span>|<span data-ttu-id="014f4-226">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="014f4-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="014f4-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="014f4-227">identityResourceIdentifier</span></span>|<span data-ttu-id="014f4-228">String</span><span class="sxs-lookup"><span data-stu-id="014f4-228">String</span></span>|<span data-ttu-id="014f4-229">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="014f4-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="014f4-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="014f4-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="014f4-231">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="014f4-231">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="014f4-232">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="014f4-232">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="014f4-233">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="014f4-233">phoneProductIdentifier</span></span>|<span data-ttu-id="014f4-234">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="014f4-234">String</span></span>|<span data-ttu-id="014f4-235">O identificador do produto de telefone.</span><span class="sxs-lookup"><span data-stu-id="014f4-235">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="014f4-236">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="014f4-236">phonePublisherId</span></span>|<span data-ttu-id="014f4-237">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="014f4-237">String</span></span>|<span data-ttu-id="014f4-238">A ID do editor do telefone.</span><span class="sxs-lookup"><span data-stu-id="014f4-238">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="014f4-239">identityVersion</span><span class="sxs-lookup"><span data-stu-id="014f4-239">identityVersion</span></span>|<span data-ttu-id="014f4-240">String</span><span class="sxs-lookup"><span data-stu-id="014f4-240">String</span></span>|<span data-ttu-id="014f4-241">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="014f4-241">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="014f4-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="014f4-242">Response</span></span>
<span data-ttu-id="014f4-243">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="014f4-243">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="014f4-244">Exemplo</span><span class="sxs-lookup"><span data-stu-id="014f4-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="014f4-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="014f4-245">Request</span></span>
<span data-ttu-id="014f4-246">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="014f4-246">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="014f4-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="014f4-247">Response</span></span>
<span data-ttu-id="014f4-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="014f4-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





