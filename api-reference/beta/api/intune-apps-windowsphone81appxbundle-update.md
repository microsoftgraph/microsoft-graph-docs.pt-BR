---
title: Atualizar windowsPhone81AppXBundle
description: Atualiza as propriedades de um objeto windowsPhone81AppXBundle.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8dd73671a1b428c053dea5b74241a1899bcc807b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157145"
---
# <a name="update-windowsphone81appxbundle"></a><span data-ttu-id="66d3a-103">Atualizar windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="66d3a-103">Update windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="66d3a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="66d3a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66d3a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="66d3a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66d3a-106">Atualiza as propriedades de um objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="66d3a-106">Update the properties of a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66d3a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="66d3a-107">Prerequisites</span></span>
<span data-ttu-id="66d3a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="66d3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="66d3a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="66d3a-110">Permission type</span></span>|<span data-ttu-id="66d3a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="66d3a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66d3a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="66d3a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66d3a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66d3a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="66d3a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="66d3a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66d3a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66d3a-115">Not supported.</span></span>|
|<span data-ttu-id="66d3a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="66d3a-116">Application</span></span>|<span data-ttu-id="66d3a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="66d3a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66d3a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="66d3a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="66d3a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="66d3a-119">Request headers</span></span>
|<span data-ttu-id="66d3a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="66d3a-120">Header</span></span>|<span data-ttu-id="66d3a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="66d3a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66d3a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="66d3a-122">Authorization</span></span>|<span data-ttu-id="66d3a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="66d3a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66d3a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="66d3a-124">Accept</span></span>|<span data-ttu-id="66d3a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="66d3a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66d3a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="66d3a-126">Request body</span></span>
<span data-ttu-id="66d3a-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) .</span><span class="sxs-lookup"><span data-stu-id="66d3a-127">In the request body, supply a JSON representation for the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

<span data-ttu-id="66d3a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span><span class="sxs-lookup"><span data-stu-id="66d3a-128">The following table shows the properties that are required when you create the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span></span>

|<span data-ttu-id="66d3a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66d3a-129">Property</span></span>|<span data-ttu-id="66d3a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="66d3a-130">Type</span></span>|<span data-ttu-id="66d3a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="66d3a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66d3a-132">id</span><span class="sxs-lookup"><span data-stu-id="66d3a-132">id</span></span>|<span data-ttu-id="66d3a-133">String</span><span class="sxs-lookup"><span data-stu-id="66d3a-133">String</span></span>|<span data-ttu-id="66d3a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="66d3a-134">Key of the entity.</span></span> <span data-ttu-id="66d3a-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66d3a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="66d3a-136">displayName</span></span>|<span data-ttu-id="66d3a-137">String</span><span class="sxs-lookup"><span data-stu-id="66d3a-137">String</span></span>|<span data-ttu-id="66d3a-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="66d3a-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="66d3a-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66d3a-140">description</span><span class="sxs-lookup"><span data-stu-id="66d3a-140">description</span></span>|<span data-ttu-id="66d3a-141">String</span><span class="sxs-lookup"><span data-stu-id="66d3a-141">String</span></span>|<span data-ttu-id="66d3a-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="66d3a-142">The description of the app.</span></span> <span data-ttu-id="66d3a-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66d3a-144">publisher</span><span class="sxs-lookup"><span data-stu-id="66d3a-144">publisher</span></span>|<span data-ttu-id="66d3a-145">String</span><span class="sxs-lookup"><span data-stu-id="66d3a-145">String</span></span>|<span data-ttu-id="66d3a-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="66d3a-146">The publisher of the app.</span></span> <span data-ttu-id="66d3a-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66d3a-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="66d3a-148">largeIcon</span></span>|[<span data-ttu-id="66d3a-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="66d3a-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="66d3a-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="66d3a-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="66d3a-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66d3a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66d3a-152">createdDateTime</span></span>|<span data-ttu-id="66d3a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66d3a-153">DateTimeOffset</span></span>|<span data-ttu-id="66d3a-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="66d3a-154">The date and time the app was created.</span></span> <span data-ttu-id="66d3a-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66d3a-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="66d3a-156">lastModifiedDateTime</span></span>|<span data-ttu-id="66d3a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66d3a-157">DateTimeOffset</span></span>|<span data-ttu-id="66d3a-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="66d3a-158">The date and time the app was last modified.</span></span> <span data-ttu-id="66d3a-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66d3a-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="66d3a-160">isFeatured</span></span>|<span data-ttu-id="66d3a-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="66d3a-161">Boolean</span></span>|<span data-ttu-id="66d3a-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66d3a-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="66d3a-163">privacyInformationUrl</span></span>|<span data-ttu-id="66d3a-164">String</span><span class="sxs-lookup"><span data-stu-id="66d3a-164">String</span></span>|<span data-ttu-id="66d3a-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="66d3a-165">The privacy statement Url.</span></span> <span data-ttu-id="66d3a-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66d3a-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="66d3a-167">informationUrl</span></span>|<span data-ttu-id="66d3a-168">String</span><span class="sxs-lookup"><span data-stu-id="66d3a-168">String</span></span>|<span data-ttu-id="66d3a-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="66d3a-169">The more information Url.</span></span> <span data-ttu-id="66d3a-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66d3a-171">owner</span><span class="sxs-lookup"><span data-stu-id="66d3a-171">owner</span></span>|<span data-ttu-id="66d3a-172">String</span><span class="sxs-lookup"><span data-stu-id="66d3a-172">String</span></span>|<span data-ttu-id="66d3a-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="66d3a-173">The owner of the app.</span></span> <span data-ttu-id="66d3a-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66d3a-175">developer</span><span class="sxs-lookup"><span data-stu-id="66d3a-175">developer</span></span>|<span data-ttu-id="66d3a-176">String</span><span class="sxs-lookup"><span data-stu-id="66d3a-176">String</span></span>|<span data-ttu-id="66d3a-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="66d3a-177">The developer of the app.</span></span> <span data-ttu-id="66d3a-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66d3a-179">Observações</span><span class="sxs-lookup"><span data-stu-id="66d3a-179">notes</span></span>|<span data-ttu-id="66d3a-180">String</span><span class="sxs-lookup"><span data-stu-id="66d3a-180">String</span></span>|<span data-ttu-id="66d3a-181">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="66d3a-181">Notes for the app.</span></span> <span data-ttu-id="66d3a-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66d3a-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="66d3a-183">uploadState</span></span>|<span data-ttu-id="66d3a-184">Int32</span><span class="sxs-lookup"><span data-stu-id="66d3a-184">Int32</span></span>|<span data-ttu-id="66d3a-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="66d3a-185">The upload state.</span></span> <span data-ttu-id="66d3a-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66d3a-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="66d3a-187">publishingState</span></span>|[<span data-ttu-id="66d3a-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="66d3a-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="66d3a-189">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="66d3a-189">The publishing state for the app.</span></span> <span data-ttu-id="66d3a-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="66d3a-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="66d3a-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="66d3a-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="66d3a-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="66d3a-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="66d3a-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="66d3a-193">isAssigned</span></span>|<span data-ttu-id="66d3a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="66d3a-194">Boolean</span></span>|<span data-ttu-id="66d3a-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="66d3a-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="66d3a-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66d3a-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="66d3a-197">roleScopeTagIds</span></span>|<span data-ttu-id="66d3a-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="66d3a-198">String collection</span></span>|<span data-ttu-id="66d3a-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="66d3a-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="66d3a-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="66d3a-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="66d3a-201">committedContentVersion</span></span>|<span data-ttu-id="66d3a-202">String</span><span class="sxs-lookup"><span data-stu-id="66d3a-202">String</span></span>|<span data-ttu-id="66d3a-203">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="66d3a-203">The internal committed content version.</span></span> <span data-ttu-id="66d3a-204">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="66d3a-205">fileName</span><span class="sxs-lookup"><span data-stu-id="66d3a-205">fileName</span></span>|<span data-ttu-id="66d3a-206">String</span><span class="sxs-lookup"><span data-stu-id="66d3a-206">String</span></span>|<span data-ttu-id="66d3a-207">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="66d3a-207">The name of the main Lob application file.</span></span> <span data-ttu-id="66d3a-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="66d3a-209">size</span><span class="sxs-lookup"><span data-stu-id="66d3a-209">size</span></span>|<span data-ttu-id="66d3a-210">Int64</span><span class="sxs-lookup"><span data-stu-id="66d3a-210">Int64</span></span>|<span data-ttu-id="66d3a-211">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="66d3a-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="66d3a-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="66d3a-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="66d3a-213">applicableArchitectures</span></span>|[<span data-ttu-id="66d3a-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="66d3a-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="66d3a-215">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="66d3a-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="66d3a-216">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span><span class="sxs-lookup"><span data-stu-id="66d3a-216">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="66d3a-217">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="66d3a-217">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="66d3a-218">identityName</span><span class="sxs-lookup"><span data-stu-id="66d3a-218">identityName</span></span>|<span data-ttu-id="66d3a-219">String</span><span class="sxs-lookup"><span data-stu-id="66d3a-219">String</span></span>|<span data-ttu-id="66d3a-220">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="66d3a-220">The Identity Name.</span></span> <span data-ttu-id="66d3a-221">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-221">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="66d3a-222">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="66d3a-222">identityPublisherHash</span></span>|<span data-ttu-id="66d3a-223">String</span><span class="sxs-lookup"><span data-stu-id="66d3a-223">String</span></span>|<span data-ttu-id="66d3a-224">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="66d3a-224">The Identity Publisher Hash.</span></span> <span data-ttu-id="66d3a-225">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-225">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="66d3a-226">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="66d3a-226">identityResourceIdentifier</span></span>|<span data-ttu-id="66d3a-227">String</span><span class="sxs-lookup"><span data-stu-id="66d3a-227">String</span></span>|<span data-ttu-id="66d3a-228">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="66d3a-228">The Identity Resource Identifier.</span></span> <span data-ttu-id="66d3a-229">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-229">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="66d3a-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="66d3a-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="66d3a-231">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="66d3a-231">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="66d3a-232">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="66d3a-232">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="66d3a-233">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-233">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="66d3a-234">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="66d3a-234">phoneProductIdentifier</span></span>|<span data-ttu-id="66d3a-235">String</span><span class="sxs-lookup"><span data-stu-id="66d3a-235">String</span></span>|<span data-ttu-id="66d3a-236">O identificador do produto de telefone.</span><span class="sxs-lookup"><span data-stu-id="66d3a-236">The Phone Product Identifier.</span></span> <span data-ttu-id="66d3a-237">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="66d3a-238">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="66d3a-238">phonePublisherId</span></span>|<span data-ttu-id="66d3a-239">String</span><span class="sxs-lookup"><span data-stu-id="66d3a-239">String</span></span>|<span data-ttu-id="66d3a-240">A ID do editor do telefone. herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-240">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="66d3a-241">identityVersion</span><span class="sxs-lookup"><span data-stu-id="66d3a-241">identityVersion</span></span>|<span data-ttu-id="66d3a-242">String</span><span class="sxs-lookup"><span data-stu-id="66d3a-242">String</span></span>|<span data-ttu-id="66d3a-243">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="66d3a-243">The identity version.</span></span> <span data-ttu-id="66d3a-244">Herdado de [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-244">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="66d3a-245">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="66d3a-245">appXPackageInformationList</span></span>|<span data-ttu-id="66d3a-246">coleção [windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)</span><span class="sxs-lookup"><span data-stu-id="66d3a-246">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="66d3a-247">A lista de informações do pacote AppX.</span><span class="sxs-lookup"><span data-stu-id="66d3a-247">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="66d3a-248">Resposta</span><span class="sxs-lookup"><span data-stu-id="66d3a-248">Response</span></span>
<span data-ttu-id="66d3a-249">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="66d3a-249">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66d3a-250">Exemplo</span><span class="sxs-lookup"><span data-stu-id="66d3a-250">Example</span></span>

### <a name="request"></a><span data-ttu-id="66d3a-251">Solicitação</span><span class="sxs-lookup"><span data-stu-id="66d3a-251">Request</span></span>
<span data-ttu-id="66d3a-252">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="66d3a-252">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2184

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
    "v10_1803": true
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
        "v10_1803": true
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="66d3a-253">Resposta</span><span class="sxs-lookup"><span data-stu-id="66d3a-253">Response</span></span>
<span data-ttu-id="66d3a-p128">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="66d3a-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2356

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
    "v10_1803": true
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
        "v10_1803": true
      }
    }
  ]
}
```




