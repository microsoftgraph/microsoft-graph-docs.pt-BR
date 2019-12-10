---
title: Atualizar windowsPhoneXAP
description: Atualiza as propriedades de um objeto windowsPhoneXAP.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8c4b18fa6fb1eb67ec9b0f3e270a7814208b2482
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39932793"
---
# <a name="update-windowsphonexap"></a><span data-ttu-id="2a0be-103">Atualizar windowsPhoneXAP</span><span class="sxs-lookup"><span data-stu-id="2a0be-103">Update windowsPhoneXAP</span></span>

> <span data-ttu-id="2a0be-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2a0be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a0be-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2a0be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a0be-106">Atualiza as propriedades de um objeto [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) .</span><span class="sxs-lookup"><span data-stu-id="2a0be-106">Update the properties of a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a0be-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2a0be-107">Prerequisites</span></span>
<span data-ttu-id="2a0be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a0be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a0be-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a0be-110">Permission type</span></span>|<span data-ttu-id="2a0be-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2a0be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a0be-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a0be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a0be-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a0be-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2a0be-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a0be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a0be-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a0be-115">Not supported.</span></span>|
|<span data-ttu-id="2a0be-116">Application</span><span class="sxs-lookup"><span data-stu-id="2a0be-116">Application</span></span>|<span data-ttu-id="2a0be-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a0be-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a0be-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a0be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="2a0be-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a0be-119">Request headers</span></span>
|<span data-ttu-id="2a0be-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2a0be-120">Header</span></span>|<span data-ttu-id="2a0be-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2a0be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a0be-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a0be-122">Authorization</span></span>|<span data-ttu-id="2a0be-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a0be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a0be-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2a0be-124">Accept</span></span>|<span data-ttu-id="2a0be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2a0be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a0be-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a0be-126">Request body</span></span>
<span data-ttu-id="2a0be-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) .</span><span class="sxs-lookup"><span data-stu-id="2a0be-127">In the request body, supply a JSON representation for the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

<span data-ttu-id="2a0be-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md).</span><span class="sxs-lookup"><span data-stu-id="2a0be-128">The following table shows the properties that are required when you create the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md).</span></span>

|<span data-ttu-id="2a0be-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2a0be-129">Property</span></span>|<span data-ttu-id="2a0be-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a0be-130">Type</span></span>|<span data-ttu-id="2a0be-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a0be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a0be-132">id</span><span class="sxs-lookup"><span data-stu-id="2a0be-132">id</span></span>|<span data-ttu-id="2a0be-133">String</span><span class="sxs-lookup"><span data-stu-id="2a0be-133">String</span></span>|<span data-ttu-id="2a0be-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2a0be-134">Key of the entity.</span></span> <span data-ttu-id="2a0be-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a0be-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2a0be-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2a0be-136">displayName</span></span>|<span data-ttu-id="2a0be-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a0be-137">String</span></span>|<span data-ttu-id="2a0be-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="2a0be-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2a0be-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a0be-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2a0be-140">description</span><span class="sxs-lookup"><span data-stu-id="2a0be-140">description</span></span>|<span data-ttu-id="2a0be-141">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2a0be-141">String</span></span>|<span data-ttu-id="2a0be-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a0be-142">The description of the app.</span></span> <span data-ttu-id="2a0be-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a0be-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2a0be-144">publicador</span><span class="sxs-lookup"><span data-stu-id="2a0be-144">publisher</span></span>|<span data-ttu-id="2a0be-145">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2a0be-145">String</span></span>|<span data-ttu-id="2a0be-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a0be-146">The publisher of the app.</span></span> <span data-ttu-id="2a0be-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a0be-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2a0be-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2a0be-148">largeIcon</span></span>|[<span data-ttu-id="2a0be-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2a0be-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2a0be-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="2a0be-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2a0be-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a0be-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2a0be-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2a0be-152">createdDateTime</span></span>|<span data-ttu-id="2a0be-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a0be-153">DateTimeOffset</span></span>|<span data-ttu-id="2a0be-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a0be-154">The date and time the app was created.</span></span> <span data-ttu-id="2a0be-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a0be-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2a0be-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a0be-156">lastModifiedDateTime</span></span>|<span data-ttu-id="2a0be-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a0be-157">DateTimeOffset</span></span>|<span data-ttu-id="2a0be-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2a0be-158">The date and time the app was last modified.</span></span> <span data-ttu-id="2a0be-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a0be-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2a0be-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2a0be-160">isFeatured</span></span>|<span data-ttu-id="2a0be-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a0be-161">Boolean</span></span>|<span data-ttu-id="2a0be-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a0be-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2a0be-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2a0be-163">privacyInformationUrl</span></span>|<span data-ttu-id="2a0be-164">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2a0be-164">String</span></span>|<span data-ttu-id="2a0be-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="2a0be-165">The privacy statement Url.</span></span> <span data-ttu-id="2a0be-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a0be-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2a0be-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2a0be-167">informationUrl</span></span>|<span data-ttu-id="2a0be-168">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2a0be-168">String</span></span>|<span data-ttu-id="2a0be-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="2a0be-169">The more information Url.</span></span> <span data-ttu-id="2a0be-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a0be-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2a0be-171">owner</span><span class="sxs-lookup"><span data-stu-id="2a0be-171">owner</span></span>|<span data-ttu-id="2a0be-172">String</span><span class="sxs-lookup"><span data-stu-id="2a0be-172">String</span></span>|<span data-ttu-id="2a0be-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="2a0be-173">The owner of the app.</span></span> <span data-ttu-id="2a0be-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a0be-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2a0be-175">developer</span><span class="sxs-lookup"><span data-stu-id="2a0be-175">developer</span></span>|<span data-ttu-id="2a0be-176">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2a0be-176">String</span></span>|<span data-ttu-id="2a0be-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a0be-177">The developer of the app.</span></span> <span data-ttu-id="2a0be-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a0be-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2a0be-179">notes</span><span class="sxs-lookup"><span data-stu-id="2a0be-179">notes</span></span>|<span data-ttu-id="2a0be-180">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2a0be-180">String</span></span>|<span data-ttu-id="2a0be-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a0be-181">Notes for the app.</span></span> <span data-ttu-id="2a0be-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a0be-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2a0be-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="2a0be-183">uploadState</span></span>|<span data-ttu-id="2a0be-184">Int32</span><span class="sxs-lookup"><span data-stu-id="2a0be-184">Int32</span></span>|<span data-ttu-id="2a0be-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="2a0be-185">The upload state.</span></span> <span data-ttu-id="2a0be-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a0be-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2a0be-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="2a0be-187">publishingState</span></span>|[<span data-ttu-id="2a0be-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2a0be-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2a0be-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a0be-189">The publishing state for the app.</span></span> <span data-ttu-id="2a0be-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="2a0be-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2a0be-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a0be-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="2a0be-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="2a0be-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2a0be-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2a0be-193">isAssigned</span></span>|<span data-ttu-id="2a0be-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a0be-194">Boolean</span></span>|<span data-ttu-id="2a0be-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="2a0be-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="2a0be-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a0be-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2a0be-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2a0be-197">roleScopeTagIds</span></span>|<span data-ttu-id="2a0be-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a0be-198">String collection</span></span>|<span data-ttu-id="2a0be-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="2a0be-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="2a0be-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a0be-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2a0be-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="2a0be-201">dependentAppCount</span></span>|<span data-ttu-id="2a0be-202">Int32</span><span class="sxs-lookup"><span data-stu-id="2a0be-202">Int32</span></span>|<span data-ttu-id="2a0be-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="2a0be-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="2a0be-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a0be-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="2a0be-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="2a0be-205">committedContentVersion</span></span>|<span data-ttu-id="2a0be-206">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2a0be-206">String</span></span>|<span data-ttu-id="2a0be-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="2a0be-207">The internal committed content version.</span></span> <span data-ttu-id="2a0be-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a0be-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2a0be-209">fileName</span><span class="sxs-lookup"><span data-stu-id="2a0be-209">fileName</span></span>|<span data-ttu-id="2a0be-210">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2a0be-210">String</span></span>|<span data-ttu-id="2a0be-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="2a0be-211">The name of the main Lob application file.</span></span> <span data-ttu-id="2a0be-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a0be-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2a0be-213">size</span><span class="sxs-lookup"><span data-stu-id="2a0be-213">size</span></span>|<span data-ttu-id="2a0be-214">Int64</span><span class="sxs-lookup"><span data-stu-id="2a0be-214">Int64</span></span>|<span data-ttu-id="2a0be-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="2a0be-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="2a0be-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a0be-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2a0be-217">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2a0be-217">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="2a0be-218">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2a0be-218">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="2a0be-219">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="2a0be-219">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="2a0be-220">productIdentifier</span><span class="sxs-lookup"><span data-stu-id="2a0be-220">productIdentifier</span></span>|<span data-ttu-id="2a0be-221">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2a0be-221">String</span></span>|<span data-ttu-id="2a0be-222">O identificador do produto.</span><span class="sxs-lookup"><span data-stu-id="2a0be-222">The Product Identifier.</span></span>|
|<span data-ttu-id="2a0be-223">identityVersion</span><span class="sxs-lookup"><span data-stu-id="2a0be-223">identityVersion</span></span>|<span data-ttu-id="2a0be-224">String</span><span class="sxs-lookup"><span data-stu-id="2a0be-224">String</span></span>|<span data-ttu-id="2a0be-225">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="2a0be-225">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="2a0be-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a0be-226">Response</span></span>
<span data-ttu-id="2a0be-227">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a0be-227">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a0be-228">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a0be-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a0be-229">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a0be-229">Request</span></span>
<span data-ttu-id="2a0be-230">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a0be-230">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1237

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
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
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="2a0be-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a0be-231">Response</span></span>
<span data-ttu-id="2a0be-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a0be-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1409

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
  "id": "301ddc77-dc77-301d-77dc-1d3077dc1d30",
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
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```





