---
title: Criar windowsPhone81AppX
description: Criar um novo objeto windowsPhone81AppX.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 678e21a2d3b662ed322dc26a07f2f110312a4ff1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166483"
---
# <a name="create-windowsphone81appx"></a><span data-ttu-id="74c16-103">Criar windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="74c16-103">Create windowsPhone81AppX</span></span>

> <span data-ttu-id="74c16-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="74c16-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74c16-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="74c16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74c16-106">Criar um novo objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) .</span><span class="sxs-lookup"><span data-stu-id="74c16-106">Create a new [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74c16-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="74c16-107">Prerequisites</span></span>
<span data-ttu-id="74c16-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="74c16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="74c16-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74c16-110">Permission type</span></span>|<span data-ttu-id="74c16-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="74c16-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74c16-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74c16-112">Delegated (work or school account)</span></span>|<span data-ttu-id="74c16-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74c16-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="74c16-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74c16-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74c16-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74c16-115">Not supported.</span></span>|
|<span data-ttu-id="74c16-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74c16-116">Application</span></span>|<span data-ttu-id="74c16-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74c16-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74c16-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74c16-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="74c16-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74c16-119">Request headers</span></span>
|<span data-ttu-id="74c16-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="74c16-120">Header</span></span>|<span data-ttu-id="74c16-121">Valor</span><span class="sxs-lookup"><span data-stu-id="74c16-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74c16-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="74c16-122">Authorization</span></span>|<span data-ttu-id="74c16-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74c16-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74c16-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="74c16-124">Accept</span></span>|<span data-ttu-id="74c16-125">application/json</span><span class="sxs-lookup"><span data-stu-id="74c16-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74c16-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74c16-126">Request body</span></span>
<span data-ttu-id="74c16-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81AppX.</span><span class="sxs-lookup"><span data-stu-id="74c16-127">In the request body, supply a JSON representation for the windowsPhone81AppX object.</span></span>

<span data-ttu-id="74c16-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81AppX.</span><span class="sxs-lookup"><span data-stu-id="74c16-128">The following table shows the properties that are required when you create the windowsPhone81AppX.</span></span>

|<span data-ttu-id="74c16-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74c16-129">Property</span></span>|<span data-ttu-id="74c16-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="74c16-130">Type</span></span>|<span data-ttu-id="74c16-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="74c16-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74c16-132">id</span><span class="sxs-lookup"><span data-stu-id="74c16-132">id</span></span>|<span data-ttu-id="74c16-133">String</span><span class="sxs-lookup"><span data-stu-id="74c16-133">String</span></span>|<span data-ttu-id="74c16-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="74c16-134">Key of the entity.</span></span> <span data-ttu-id="74c16-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="74c16-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="74c16-136">displayName</span><span class="sxs-lookup"><span data-stu-id="74c16-136">displayName</span></span>|<span data-ttu-id="74c16-137">String</span><span class="sxs-lookup"><span data-stu-id="74c16-137">String</span></span>|<span data-ttu-id="74c16-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="74c16-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="74c16-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="74c16-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="74c16-140">description</span><span class="sxs-lookup"><span data-stu-id="74c16-140">description</span></span>|<span data-ttu-id="74c16-141">String</span><span class="sxs-lookup"><span data-stu-id="74c16-141">String</span></span>|<span data-ttu-id="74c16-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="74c16-142">The description of the app.</span></span> <span data-ttu-id="74c16-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="74c16-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="74c16-144">publisher</span><span class="sxs-lookup"><span data-stu-id="74c16-144">publisher</span></span>|<span data-ttu-id="74c16-145">String</span><span class="sxs-lookup"><span data-stu-id="74c16-145">String</span></span>|<span data-ttu-id="74c16-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="74c16-146">The publisher of the app.</span></span> <span data-ttu-id="74c16-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="74c16-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="74c16-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="74c16-148">largeIcon</span></span>|[<span data-ttu-id="74c16-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="74c16-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="74c16-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="74c16-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="74c16-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="74c16-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="74c16-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="74c16-152">createdDateTime</span></span>|<span data-ttu-id="74c16-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74c16-153">DateTimeOffset</span></span>|<span data-ttu-id="74c16-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="74c16-154">The date and time the app was created.</span></span> <span data-ttu-id="74c16-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="74c16-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="74c16-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="74c16-156">lastModifiedDateTime</span></span>|<span data-ttu-id="74c16-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74c16-157">DateTimeOffset</span></span>|<span data-ttu-id="74c16-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="74c16-158">The date and time the app was last modified.</span></span> <span data-ttu-id="74c16-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="74c16-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="74c16-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="74c16-160">isFeatured</span></span>|<span data-ttu-id="74c16-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="74c16-161">Boolean</span></span>|<span data-ttu-id="74c16-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="74c16-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="74c16-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="74c16-163">privacyInformationUrl</span></span>|<span data-ttu-id="74c16-164">String</span><span class="sxs-lookup"><span data-stu-id="74c16-164">String</span></span>|<span data-ttu-id="74c16-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="74c16-165">The privacy statement Url.</span></span> <span data-ttu-id="74c16-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="74c16-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="74c16-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="74c16-167">informationUrl</span></span>|<span data-ttu-id="74c16-168">String</span><span class="sxs-lookup"><span data-stu-id="74c16-168">String</span></span>|<span data-ttu-id="74c16-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="74c16-169">The more information Url.</span></span> <span data-ttu-id="74c16-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="74c16-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="74c16-171">owner</span><span class="sxs-lookup"><span data-stu-id="74c16-171">owner</span></span>|<span data-ttu-id="74c16-172">String</span><span class="sxs-lookup"><span data-stu-id="74c16-172">String</span></span>|<span data-ttu-id="74c16-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="74c16-173">The owner of the app.</span></span> <span data-ttu-id="74c16-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="74c16-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="74c16-175">developer</span><span class="sxs-lookup"><span data-stu-id="74c16-175">developer</span></span>|<span data-ttu-id="74c16-176">String</span><span class="sxs-lookup"><span data-stu-id="74c16-176">String</span></span>|<span data-ttu-id="74c16-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="74c16-177">The developer of the app.</span></span> <span data-ttu-id="74c16-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="74c16-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="74c16-179">Observações</span><span class="sxs-lookup"><span data-stu-id="74c16-179">notes</span></span>|<span data-ttu-id="74c16-180">String</span><span class="sxs-lookup"><span data-stu-id="74c16-180">String</span></span>|<span data-ttu-id="74c16-181">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="74c16-181">Notes for the app.</span></span> <span data-ttu-id="74c16-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="74c16-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="74c16-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="74c16-183">uploadState</span></span>|<span data-ttu-id="74c16-184">Int32</span><span class="sxs-lookup"><span data-stu-id="74c16-184">Int32</span></span>|<span data-ttu-id="74c16-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="74c16-185">The upload state.</span></span> <span data-ttu-id="74c16-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="74c16-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="74c16-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="74c16-187">publishingState</span></span>|[<span data-ttu-id="74c16-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="74c16-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="74c16-189">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="74c16-189">The publishing state for the app.</span></span> <span data-ttu-id="74c16-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="74c16-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="74c16-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="74c16-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="74c16-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="74c16-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="74c16-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="74c16-193">isAssigned</span></span>|<span data-ttu-id="74c16-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="74c16-194">Boolean</span></span>|<span data-ttu-id="74c16-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="74c16-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="74c16-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="74c16-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="74c16-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="74c16-197">roleScopeTagIds</span></span>|<span data-ttu-id="74c16-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="74c16-198">String collection</span></span>|<span data-ttu-id="74c16-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="74c16-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="74c16-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="74c16-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="74c16-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="74c16-201">committedContentVersion</span></span>|<span data-ttu-id="74c16-202">String</span><span class="sxs-lookup"><span data-stu-id="74c16-202">String</span></span>|<span data-ttu-id="74c16-203">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="74c16-203">The internal committed content version.</span></span> <span data-ttu-id="74c16-204">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="74c16-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="74c16-205">fileName</span><span class="sxs-lookup"><span data-stu-id="74c16-205">fileName</span></span>|<span data-ttu-id="74c16-206">String</span><span class="sxs-lookup"><span data-stu-id="74c16-206">String</span></span>|<span data-ttu-id="74c16-207">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="74c16-207">The name of the main Lob application file.</span></span> <span data-ttu-id="74c16-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="74c16-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="74c16-209">size</span><span class="sxs-lookup"><span data-stu-id="74c16-209">size</span></span>|<span data-ttu-id="74c16-210">Int64</span><span class="sxs-lookup"><span data-stu-id="74c16-210">Int64</span></span>|<span data-ttu-id="74c16-211">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="74c16-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="74c16-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="74c16-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="74c16-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="74c16-213">applicableArchitectures</span></span>|[<span data-ttu-id="74c16-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="74c16-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="74c16-215">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="74c16-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="74c16-216">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="74c16-216">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="74c16-217">identityName</span><span class="sxs-lookup"><span data-stu-id="74c16-217">identityName</span></span>|<span data-ttu-id="74c16-218">String</span><span class="sxs-lookup"><span data-stu-id="74c16-218">String</span></span>|<span data-ttu-id="74c16-219">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="74c16-219">The Identity Name.</span></span>|
|<span data-ttu-id="74c16-220">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="74c16-220">identityPublisherHash</span></span>|<span data-ttu-id="74c16-221">String</span><span class="sxs-lookup"><span data-stu-id="74c16-221">String</span></span>|<span data-ttu-id="74c16-222">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="74c16-222">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="74c16-223">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="74c16-223">identityResourceIdentifier</span></span>|<span data-ttu-id="74c16-224">String</span><span class="sxs-lookup"><span data-stu-id="74c16-224">String</span></span>|<span data-ttu-id="74c16-225">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="74c16-225">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="74c16-226">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="74c16-226">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="74c16-227">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="74c16-227">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="74c16-228">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="74c16-228">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="74c16-229">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="74c16-229">phoneProductIdentifier</span></span>|<span data-ttu-id="74c16-230">String</span><span class="sxs-lookup"><span data-stu-id="74c16-230">String</span></span>|<span data-ttu-id="74c16-231">O identificador do produto de telefone.</span><span class="sxs-lookup"><span data-stu-id="74c16-231">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="74c16-232">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="74c16-232">phonePublisherId</span></span>|<span data-ttu-id="74c16-233">String</span><span class="sxs-lookup"><span data-stu-id="74c16-233">String</span></span>|<span data-ttu-id="74c16-234">A ID do editor do telefone.</span><span class="sxs-lookup"><span data-stu-id="74c16-234">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="74c16-235">identityVersion</span><span class="sxs-lookup"><span data-stu-id="74c16-235">identityVersion</span></span>|<span data-ttu-id="74c16-236">String</span><span class="sxs-lookup"><span data-stu-id="74c16-236">String</span></span>|<span data-ttu-id="74c16-237">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="74c16-237">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="74c16-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="74c16-238">Response</span></span>
<span data-ttu-id="74c16-239">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74c16-239">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74c16-240">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74c16-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="74c16-241">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74c16-241">Request</span></span>
<span data-ttu-id="74c16-242">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="74c16-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1440

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
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="74c16-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="74c16-243">Response</span></span>
<span data-ttu-id="74c16-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74c16-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1612

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
  "identityVersion": "Identity Version value"
}
```




