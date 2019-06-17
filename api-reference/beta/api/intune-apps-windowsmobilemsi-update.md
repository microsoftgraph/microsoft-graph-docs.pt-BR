---
title: Atualizar windowsMobileMSI
description: Atualiza as propriedades de um objeto windowsMobileMSI.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ce050708c81ea81c6acf7669aae64341c232f1f1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34973107"
---
# <a name="update-windowsmobilemsi"></a><span data-ttu-id="11337-103">Atualizar windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="11337-103">Update windowsMobileMSI</span></span>

> <span data-ttu-id="11337-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="11337-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11337-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="11337-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11337-106">Atualiza as propriedades de um objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="11337-106">Update the properties of a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11337-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="11337-107">Prerequisites</span></span>
<span data-ttu-id="11337-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11337-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11337-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11337-110">Permission type</span></span>|<span data-ttu-id="11337-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="11337-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11337-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11337-112">Delegated (work or school account)</span></span>|<span data-ttu-id="11337-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11337-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="11337-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11337-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11337-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11337-115">Not supported.</span></span>|
|<span data-ttu-id="11337-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11337-116">Application</span></span>|<span data-ttu-id="11337-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11337-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11337-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11337-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="11337-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11337-119">Request headers</span></span>
|<span data-ttu-id="11337-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="11337-120">Header</span></span>|<span data-ttu-id="11337-121">Valor</span><span class="sxs-lookup"><span data-stu-id="11337-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11337-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="11337-122">Authorization</span></span>|<span data-ttu-id="11337-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11337-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11337-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="11337-124">Accept</span></span>|<span data-ttu-id="11337-125">application/json</span><span class="sxs-lookup"><span data-stu-id="11337-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11337-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11337-126">Request body</span></span>
<span data-ttu-id="11337-127">No corpo da solicitação, forneça uma representação JSON para o objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="11337-127">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="11337-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="11337-128">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

|<span data-ttu-id="11337-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11337-129">Property</span></span>|<span data-ttu-id="11337-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="11337-130">Type</span></span>|<span data-ttu-id="11337-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="11337-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11337-132">id</span><span class="sxs-lookup"><span data-stu-id="11337-132">id</span></span>|<span data-ttu-id="11337-133">String</span><span class="sxs-lookup"><span data-stu-id="11337-133">String</span></span>|<span data-ttu-id="11337-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="11337-134">Key of the entity.</span></span> <span data-ttu-id="11337-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11337-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11337-136">displayName</span><span class="sxs-lookup"><span data-stu-id="11337-136">displayName</span></span>|<span data-ttu-id="11337-137">String</span><span class="sxs-lookup"><span data-stu-id="11337-137">String</span></span>|<span data-ttu-id="11337-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="11337-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="11337-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11337-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11337-140">descrição</span><span class="sxs-lookup"><span data-stu-id="11337-140">description</span></span>|<span data-ttu-id="11337-141">String</span><span class="sxs-lookup"><span data-stu-id="11337-141">String</span></span>|<span data-ttu-id="11337-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11337-142">The description of the app.</span></span> <span data-ttu-id="11337-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11337-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11337-144">publicador</span><span class="sxs-lookup"><span data-stu-id="11337-144">publisher</span></span>|<span data-ttu-id="11337-145">String</span><span class="sxs-lookup"><span data-stu-id="11337-145">String</span></span>|<span data-ttu-id="11337-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11337-146">The publisher of the app.</span></span> <span data-ttu-id="11337-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11337-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11337-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="11337-148">largeIcon</span></span>|[<span data-ttu-id="11337-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="11337-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="11337-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="11337-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="11337-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11337-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11337-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11337-152">createdDateTime</span></span>|<span data-ttu-id="11337-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11337-153">DateTimeOffset</span></span>|<span data-ttu-id="11337-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11337-154">The date and time the app was created.</span></span> <span data-ttu-id="11337-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11337-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11337-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11337-156">lastModifiedDateTime</span></span>|<span data-ttu-id="11337-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11337-157">DateTimeOffset</span></span>|<span data-ttu-id="11337-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="11337-158">The date and time the app was last modified.</span></span> <span data-ttu-id="11337-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11337-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11337-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="11337-160">isFeatured</span></span>|<span data-ttu-id="11337-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="11337-161">Boolean</span></span>|<span data-ttu-id="11337-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11337-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11337-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="11337-163">privacyInformationUrl</span></span>|<span data-ttu-id="11337-164">String</span><span class="sxs-lookup"><span data-stu-id="11337-164">String</span></span>|<span data-ttu-id="11337-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="11337-165">The privacy statement Url.</span></span> <span data-ttu-id="11337-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11337-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11337-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="11337-167">informationUrl</span></span>|<span data-ttu-id="11337-168">String</span><span class="sxs-lookup"><span data-stu-id="11337-168">String</span></span>|<span data-ttu-id="11337-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="11337-169">The more information Url.</span></span> <span data-ttu-id="11337-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11337-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11337-171">owner</span><span class="sxs-lookup"><span data-stu-id="11337-171">owner</span></span>|<span data-ttu-id="11337-172">String</span><span class="sxs-lookup"><span data-stu-id="11337-172">String</span></span>|<span data-ttu-id="11337-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="11337-173">The owner of the app.</span></span> <span data-ttu-id="11337-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11337-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11337-175">developer</span><span class="sxs-lookup"><span data-stu-id="11337-175">developer</span></span>|<span data-ttu-id="11337-176">String</span><span class="sxs-lookup"><span data-stu-id="11337-176">String</span></span>|<span data-ttu-id="11337-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11337-177">The developer of the app.</span></span> <span data-ttu-id="11337-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11337-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11337-179">notes</span><span class="sxs-lookup"><span data-stu-id="11337-179">notes</span></span>|<span data-ttu-id="11337-180">String</span><span class="sxs-lookup"><span data-stu-id="11337-180">String</span></span>|<span data-ttu-id="11337-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11337-181">Notes for the app.</span></span> <span data-ttu-id="11337-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11337-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11337-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="11337-183">uploadState</span></span>|<span data-ttu-id="11337-184">Int32</span><span class="sxs-lookup"><span data-stu-id="11337-184">Int32</span></span>|<span data-ttu-id="11337-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="11337-185">The upload state.</span></span> <span data-ttu-id="11337-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11337-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11337-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="11337-187">publishingState</span></span>|[<span data-ttu-id="11337-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="11337-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="11337-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11337-189">The publishing state for the app.</span></span> <span data-ttu-id="11337-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="11337-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="11337-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="11337-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="11337-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="11337-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="11337-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="11337-193">isAssigned</span></span>|<span data-ttu-id="11337-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="11337-194">Boolean</span></span>|<span data-ttu-id="11337-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="11337-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="11337-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11337-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11337-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="11337-197">roleScopeTagIds</span></span>|<span data-ttu-id="11337-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="11337-198">String collection</span></span>|<span data-ttu-id="11337-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="11337-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="11337-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11337-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11337-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="11337-201">dependentAppCount</span></span>|<span data-ttu-id="11337-202">Int32</span><span class="sxs-lookup"><span data-stu-id="11337-202">Int32</span></span>|<span data-ttu-id="11337-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="11337-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="11337-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="11337-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="11337-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="11337-205">committedContentVersion</span></span>|<span data-ttu-id="11337-206">String</span><span class="sxs-lookup"><span data-stu-id="11337-206">String</span></span>|<span data-ttu-id="11337-207">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="11337-207">The internal committed content version.</span></span> <span data-ttu-id="11337-208">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="11337-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="11337-209">fileName</span><span class="sxs-lookup"><span data-stu-id="11337-209">fileName</span></span>|<span data-ttu-id="11337-210">String</span><span class="sxs-lookup"><span data-stu-id="11337-210">String</span></span>|<span data-ttu-id="11337-211">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="11337-211">The name of the main Lob application file.</span></span> <span data-ttu-id="11337-212">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="11337-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="11337-213">size</span><span class="sxs-lookup"><span data-stu-id="11337-213">size</span></span>|<span data-ttu-id="11337-214">Int64</span><span class="sxs-lookup"><span data-stu-id="11337-214">Int64</span></span>|<span data-ttu-id="11337-215">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="11337-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="11337-216">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="11337-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="11337-217">commandLine</span><span class="sxs-lookup"><span data-stu-id="11337-217">commandLine</span></span>|<span data-ttu-id="11337-218">String</span><span class="sxs-lookup"><span data-stu-id="11337-218">String</span></span>|<span data-ttu-id="11337-219">A linha de comando.</span><span class="sxs-lookup"><span data-stu-id="11337-219">The command line.</span></span>|
|<span data-ttu-id="11337-220">productCode</span><span class="sxs-lookup"><span data-stu-id="11337-220">productCode</span></span>|<span data-ttu-id="11337-221">String</span><span class="sxs-lookup"><span data-stu-id="11337-221">String</span></span>|<span data-ttu-id="11337-222">O código do produto.</span><span class="sxs-lookup"><span data-stu-id="11337-222">The product code.</span></span>|
|<span data-ttu-id="11337-223">productVersion</span><span class="sxs-lookup"><span data-stu-id="11337-223">productVersion</span></span>|<span data-ttu-id="11337-224">String</span><span class="sxs-lookup"><span data-stu-id="11337-224">String</span></span>|<span data-ttu-id="11337-225">A versão de produto do aplicativo de linha de negócios (LoB) Windows Mobile MSI.</span><span class="sxs-lookup"><span data-stu-id="11337-225">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="11337-226">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="11337-226">ignoreVersionDetection</span></span>|<span data-ttu-id="11337-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="11337-227">Boolean</span></span>|<span data-ttu-id="11337-228">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="11337-228">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="11337-229">Defina como true para o aplicativos de linha de negócios (LoB) Windows Mobile MSI que usam um recurso de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="11337-229">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="11337-230">identityVersion</span><span class="sxs-lookup"><span data-stu-id="11337-230">identityVersion</span></span>|<span data-ttu-id="11337-231">String</span><span class="sxs-lookup"><span data-stu-id="11337-231">String</span></span>|<span data-ttu-id="11337-232">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="11337-232">The identity version.</span></span>|
|<span data-ttu-id="11337-233">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="11337-233">useDeviceContext</span></span>|<span data-ttu-id="11337-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="11337-234">Boolean</span></span>|<span data-ttu-id="11337-235">Indica se um MSI de modo duplo deve ser instalado no contexto de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="11337-235">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="11337-236">Se true, o aplicativo será instalado para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="11337-236">If true, app will be installed for all users.</span></span> <span data-ttu-id="11337-237">Se false, o aplicativo será instalado por usuário.</span><span class="sxs-lookup"><span data-stu-id="11337-237">If false, app will be installed per-user.</span></span> <span data-ttu-id="11337-238">Se for NULL, o serviço usará o contexto de instalação padrão do pacote MSI.</span><span class="sxs-lookup"><span data-stu-id="11337-238">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="11337-239">No caso do MSI de modo duplo, esse padrão será por usuário.</span><span class="sxs-lookup"><span data-stu-id="11337-239">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="11337-240">Não pode ser definido para aplicativos de modo não duplo.</span><span class="sxs-lookup"><span data-stu-id="11337-240">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="11337-241">Não pode ser alterado após a criação inicial do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="11337-241">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="11337-242">Resposta</span><span class="sxs-lookup"><span data-stu-id="11337-242">Response</span></span>
<span data-ttu-id="11337-243">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11337-243">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11337-244">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11337-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="11337-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11337-245">Request</span></span>
<span data-ttu-id="11337-246">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="11337-246">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1066

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```

### <a name="response"></a><span data-ttu-id="11337-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="11337-247">Response</span></span>
<span data-ttu-id="11337-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11337-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1238

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```





