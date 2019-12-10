---
title: Atualizar windowsPhone81AppXBundle
description: Atualiza as propriedades de um objeto windowsPhone81AppXBundle.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: be48a0c7228492b25459c90c039535760bdd8020
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39933136"
---
# <a name="update-windowsphone81appxbundle"></a><span data-ttu-id="53c86-103">Atualizar windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="53c86-103">Update windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="53c86-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="53c86-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53c86-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="53c86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53c86-106">Atualiza as propriedades de um objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="53c86-106">Update the properties of a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53c86-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="53c86-107">Prerequisites</span></span>
<span data-ttu-id="53c86-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53c86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53c86-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53c86-110">Permission type</span></span>|<span data-ttu-id="53c86-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="53c86-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53c86-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53c86-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53c86-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53c86-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="53c86-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53c86-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53c86-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53c86-115">Not supported.</span></span>|
|<span data-ttu-id="53c86-116">Application</span><span class="sxs-lookup"><span data-stu-id="53c86-116">Application</span></span>|<span data-ttu-id="53c86-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53c86-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53c86-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53c86-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="53c86-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53c86-119">Request headers</span></span>
|<span data-ttu-id="53c86-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="53c86-120">Header</span></span>|<span data-ttu-id="53c86-121">Valor</span><span class="sxs-lookup"><span data-stu-id="53c86-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53c86-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="53c86-122">Authorization</span></span>|<span data-ttu-id="53c86-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53c86-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53c86-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="53c86-124">Accept</span></span>|<span data-ttu-id="53c86-125">application/json</span><span class="sxs-lookup"><span data-stu-id="53c86-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53c86-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53c86-126">Request body</span></span>
<span data-ttu-id="53c86-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="53c86-127">In the request body, supply a JSON representation for the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

<span data-ttu-id="53c86-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span><span class="sxs-lookup"><span data-stu-id="53c86-128">The following table shows the properties that are required when you create the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span></span>

|<span data-ttu-id="53c86-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53c86-129">Property</span></span>|<span data-ttu-id="53c86-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="53c86-130">Type</span></span>|<span data-ttu-id="53c86-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="53c86-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53c86-132">id</span><span class="sxs-lookup"><span data-stu-id="53c86-132">id</span></span>|<span data-ttu-id="53c86-133">String</span><span class="sxs-lookup"><span data-stu-id="53c86-133">String</span></span>|<span data-ttu-id="53c86-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="53c86-134">Key of the entity.</span></span> <span data-ttu-id="53c86-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53c86-136">displayName</span><span class="sxs-lookup"><span data-stu-id="53c86-136">displayName</span></span>|<span data-ttu-id="53c86-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53c86-137">String</span></span>|<span data-ttu-id="53c86-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="53c86-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="53c86-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53c86-140">description</span><span class="sxs-lookup"><span data-stu-id="53c86-140">description</span></span>|<span data-ttu-id="53c86-141">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="53c86-141">String</span></span>|<span data-ttu-id="53c86-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53c86-142">The description of the app.</span></span> <span data-ttu-id="53c86-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53c86-144">publicador</span><span class="sxs-lookup"><span data-stu-id="53c86-144">publisher</span></span>|<span data-ttu-id="53c86-145">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="53c86-145">String</span></span>|<span data-ttu-id="53c86-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53c86-146">The publisher of the app.</span></span> <span data-ttu-id="53c86-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53c86-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="53c86-148">largeIcon</span></span>|[<span data-ttu-id="53c86-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="53c86-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="53c86-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="53c86-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="53c86-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53c86-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="53c86-152">createdDateTime</span></span>|<span data-ttu-id="53c86-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53c86-153">DateTimeOffset</span></span>|<span data-ttu-id="53c86-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53c86-154">The date and time the app was created.</span></span> <span data-ttu-id="53c86-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53c86-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53c86-156">lastModifiedDateTime</span></span>|<span data-ttu-id="53c86-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53c86-157">DateTimeOffset</span></span>|<span data-ttu-id="53c86-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="53c86-158">The date and time the app was last modified.</span></span> <span data-ttu-id="53c86-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53c86-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="53c86-160">isFeatured</span></span>|<span data-ttu-id="53c86-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="53c86-161">Boolean</span></span>|<span data-ttu-id="53c86-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53c86-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="53c86-163">privacyInformationUrl</span></span>|<span data-ttu-id="53c86-164">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="53c86-164">String</span></span>|<span data-ttu-id="53c86-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="53c86-165">The privacy statement Url.</span></span> <span data-ttu-id="53c86-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53c86-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="53c86-167">informationUrl</span></span>|<span data-ttu-id="53c86-168">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="53c86-168">String</span></span>|<span data-ttu-id="53c86-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="53c86-169">The more information Url.</span></span> <span data-ttu-id="53c86-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53c86-171">owner</span><span class="sxs-lookup"><span data-stu-id="53c86-171">owner</span></span>|<span data-ttu-id="53c86-172">String</span><span class="sxs-lookup"><span data-stu-id="53c86-172">String</span></span>|<span data-ttu-id="53c86-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="53c86-173">The owner of the app.</span></span> <span data-ttu-id="53c86-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53c86-175">developer</span><span class="sxs-lookup"><span data-stu-id="53c86-175">developer</span></span>|<span data-ttu-id="53c86-176">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="53c86-176">String</span></span>|<span data-ttu-id="53c86-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53c86-177">The developer of the app.</span></span> <span data-ttu-id="53c86-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53c86-179">notes</span><span class="sxs-lookup"><span data-stu-id="53c86-179">notes</span></span>|<span data-ttu-id="53c86-180">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="53c86-180">String</span></span>|<span data-ttu-id="53c86-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53c86-181">Notes for the app.</span></span> <span data-ttu-id="53c86-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53c86-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="53c86-183">uploadState</span></span>|<span data-ttu-id="53c86-184">Int32</span><span class="sxs-lookup"><span data-stu-id="53c86-184">Int32</span></span>|<span data-ttu-id="53c86-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="53c86-185">The upload state.</span></span> <span data-ttu-id="53c86-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53c86-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="53c86-187">publishingState</span></span>|[<span data-ttu-id="53c86-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="53c86-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="53c86-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53c86-189">The publishing state for the app.</span></span> <span data-ttu-id="53c86-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="53c86-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="53c86-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="53c86-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="53c86-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="53c86-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="53c86-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="53c86-193">isAssigned</span></span>|<span data-ttu-id="53c86-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="53c86-194">Boolean</span></span>|<span data-ttu-id="53c86-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="53c86-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="53c86-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53c86-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="53c86-197">roleScopeTagIds</span></span>|<span data-ttu-id="53c86-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="53c86-198">String collection</span></span>|<span data-ttu-id="53c86-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="53c86-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="53c86-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53c86-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="53c86-201">dependentAppCount</span></span>|<span data-ttu-id="53c86-202">Int32</span><span class="sxs-lookup"><span data-stu-id="53c86-202">Int32</span></span>|<span data-ttu-id="53c86-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="53c86-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="53c86-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="53c86-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="53c86-205">committedContentVersion</span></span>|<span data-ttu-id="53c86-206">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="53c86-206">String</span></span>|<span data-ttu-id="53c86-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="53c86-207">The internal committed content version.</span></span> <span data-ttu-id="53c86-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="53c86-209">fileName</span><span class="sxs-lookup"><span data-stu-id="53c86-209">fileName</span></span>|<span data-ttu-id="53c86-210">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="53c86-210">String</span></span>|<span data-ttu-id="53c86-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="53c86-211">The name of the main Lob application file.</span></span> <span data-ttu-id="53c86-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="53c86-213">size</span><span class="sxs-lookup"><span data-stu-id="53c86-213">size</span></span>|<span data-ttu-id="53c86-214">Int64</span><span class="sxs-lookup"><span data-stu-id="53c86-214">Int64</span></span>|<span data-ttu-id="53c86-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="53c86-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="53c86-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="53c86-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="53c86-217">applicableArchitectures</span></span>|[<span data-ttu-id="53c86-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="53c86-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="53c86-219">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="53c86-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="53c86-220">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="53c86-220">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="53c86-221">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="53c86-221">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="53c86-222">identityName</span><span class="sxs-lookup"><span data-stu-id="53c86-222">identityName</span></span>|<span data-ttu-id="53c86-223">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="53c86-223">String</span></span>|<span data-ttu-id="53c86-224">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="53c86-224">The Identity Name.</span></span> <span data-ttu-id="53c86-225">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-225">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="53c86-226">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="53c86-226">identityPublisherHash</span></span>|<span data-ttu-id="53c86-227">String</span><span class="sxs-lookup"><span data-stu-id="53c86-227">String</span></span>|<span data-ttu-id="53c86-228">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="53c86-228">The Identity Publisher Hash.</span></span> <span data-ttu-id="53c86-229">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-229">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="53c86-230">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="53c86-230">identityResourceIdentifier</span></span>|<span data-ttu-id="53c86-231">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="53c86-231">String</span></span>|<span data-ttu-id="53c86-232">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="53c86-232">The Identity Resource Identifier.</span></span> <span data-ttu-id="53c86-233">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-233">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="53c86-234">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="53c86-234">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="53c86-235">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="53c86-235">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="53c86-236">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="53c86-236">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="53c86-237">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="53c86-238">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="53c86-238">phoneProductIdentifier</span></span>|<span data-ttu-id="53c86-239">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="53c86-239">String</span></span>|<span data-ttu-id="53c86-240">O identificador do produto de telefone.</span><span class="sxs-lookup"><span data-stu-id="53c86-240">The Phone Product Identifier.</span></span> <span data-ttu-id="53c86-241">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-241">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="53c86-242">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="53c86-242">phonePublisherId</span></span>|<span data-ttu-id="53c86-243">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="53c86-243">String</span></span>|<span data-ttu-id="53c86-244">A ID do editor do telefone. herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-244">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="53c86-245">identityVersion</span><span class="sxs-lookup"><span data-stu-id="53c86-245">identityVersion</span></span>|<span data-ttu-id="53c86-246">String</span><span class="sxs-lookup"><span data-stu-id="53c86-246">String</span></span>|<span data-ttu-id="53c86-247">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="53c86-247">The identity version.</span></span> <span data-ttu-id="53c86-248">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-248">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="53c86-249">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="53c86-249">appXPackageInformationList</span></span>|<span data-ttu-id="53c86-250">coleção [windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)</span><span class="sxs-lookup"><span data-stu-id="53c86-250">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="53c86-251">A lista de informações do pacote AppX.</span><span class="sxs-lookup"><span data-stu-id="53c86-251">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="53c86-252">Resposta</span><span class="sxs-lookup"><span data-stu-id="53c86-252">Response</span></span>
<span data-ttu-id="53c86-253">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53c86-253">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53c86-254">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53c86-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="53c86-255">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53c86-255">Request</span></span>
<span data-ttu-id="53c86-256">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53c86-256">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2311

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
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
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
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
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="53c86-257">Resposta</span><span class="sxs-lookup"><span data-stu-id="53c86-257">Response</span></span>
<span data-ttu-id="53c86-p129">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53c86-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2483

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
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
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
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
      }
    }
  ]
}
```





