---
title: Atualizar windowsMobileMSI
description: Atualiza as propriedades de um objeto windowsMobileMSI.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cff6787f782c4c86cbcc9298c0205e75315614dd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950897"
---
# <a name="update-windowsmobilemsi"></a><span data-ttu-id="828a3-103">Atualizar windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="828a3-103">Update windowsMobileMSI</span></span>

> <span data-ttu-id="828a3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="828a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="828a3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="828a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="828a3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="828a3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="828a3-107">Atualiza as propriedades de um objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="828a3-107">Update the properties of a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="828a3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="828a3-108">Prerequisites</span></span>
<span data-ttu-id="828a3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="828a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="828a3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="828a3-111">Permission type</span></span>|<span data-ttu-id="828a3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="828a3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="828a3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="828a3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="828a3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="828a3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="828a3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="828a3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="828a3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="828a3-116">Not supported.</span></span>|
|<span data-ttu-id="828a3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="828a3-117">Application</span></span>|<span data-ttu-id="828a3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="828a3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="828a3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="828a3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="828a3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="828a3-120">Request headers</span></span>
|<span data-ttu-id="828a3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="828a3-121">Header</span></span>|<span data-ttu-id="828a3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="828a3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="828a3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="828a3-123">Authorization</span></span>|<span data-ttu-id="828a3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="828a3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="828a3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="828a3-125">Accept</span></span>|<span data-ttu-id="828a3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="828a3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="828a3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="828a3-127">Request body</span></span>
<span data-ttu-id="828a3-128">No corpo da solicitação, forneça uma representação JSON para o objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="828a3-128">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="828a3-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="828a3-129">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

|<span data-ttu-id="828a3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="828a3-130">Property</span></span>|<span data-ttu-id="828a3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="828a3-131">Type</span></span>|<span data-ttu-id="828a3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="828a3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="828a3-133">id</span><span class="sxs-lookup"><span data-stu-id="828a3-133">id</span></span>|<span data-ttu-id="828a3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="828a3-134">String</span></span>|<span data-ttu-id="828a3-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="828a3-135">Key of the entity.</span></span> <span data-ttu-id="828a3-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="828a3-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="828a3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="828a3-137">displayName</span></span>|<span data-ttu-id="828a3-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="828a3-138">String</span></span>|<span data-ttu-id="828a3-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="828a3-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="828a3-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="828a3-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="828a3-141">description</span><span class="sxs-lookup"><span data-stu-id="828a3-141">description</span></span>|<span data-ttu-id="828a3-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="828a3-142">String</span></span>|<span data-ttu-id="828a3-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="828a3-143">The description of the app.</span></span> <span data-ttu-id="828a3-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="828a3-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="828a3-145">publisher</span><span class="sxs-lookup"><span data-stu-id="828a3-145">publisher</span></span>|<span data-ttu-id="828a3-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="828a3-146">String</span></span>|<span data-ttu-id="828a3-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="828a3-147">The publisher of the app.</span></span> <span data-ttu-id="828a3-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="828a3-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="828a3-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="828a3-149">largeIcon</span></span>|[<span data-ttu-id="828a3-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="828a3-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="828a3-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="828a3-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="828a3-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="828a3-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="828a3-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="828a3-153">createdDateTime</span></span>|<span data-ttu-id="828a3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="828a3-154">DateTimeOffset</span></span>|<span data-ttu-id="828a3-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="828a3-155">The date and time the app was created.</span></span> <span data-ttu-id="828a3-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="828a3-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="828a3-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="828a3-157">lastModifiedDateTime</span></span>|<span data-ttu-id="828a3-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="828a3-158">DateTimeOffset</span></span>|<span data-ttu-id="828a3-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="828a3-159">The date and time the app was last modified.</span></span> <span data-ttu-id="828a3-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="828a3-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="828a3-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="828a3-161">isFeatured</span></span>|<span data-ttu-id="828a3-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="828a3-162">Boolean</span></span>|<span data-ttu-id="828a3-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="828a3-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="828a3-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="828a3-164">privacyInformationUrl</span></span>|<span data-ttu-id="828a3-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="828a3-165">String</span></span>|<span data-ttu-id="828a3-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="828a3-166">The privacy statement Url.</span></span> <span data-ttu-id="828a3-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="828a3-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="828a3-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="828a3-168">informationUrl</span></span>|<span data-ttu-id="828a3-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="828a3-169">String</span></span>|<span data-ttu-id="828a3-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="828a3-170">The more information Url.</span></span> <span data-ttu-id="828a3-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="828a3-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="828a3-172">owner</span><span class="sxs-lookup"><span data-stu-id="828a3-172">owner</span></span>|<span data-ttu-id="828a3-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="828a3-173">String</span></span>|<span data-ttu-id="828a3-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="828a3-174">The owner of the app.</span></span> <span data-ttu-id="828a3-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="828a3-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="828a3-176">developer</span><span class="sxs-lookup"><span data-stu-id="828a3-176">developer</span></span>|<span data-ttu-id="828a3-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="828a3-177">String</span></span>|<span data-ttu-id="828a3-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="828a3-178">The developer of the app.</span></span> <span data-ttu-id="828a3-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="828a3-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="828a3-180">Observações</span><span class="sxs-lookup"><span data-stu-id="828a3-180">notes</span></span>|<span data-ttu-id="828a3-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="828a3-181">String</span></span>|<span data-ttu-id="828a3-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="828a3-182">Notes for the app.</span></span> <span data-ttu-id="828a3-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="828a3-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="828a3-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="828a3-184">uploadState</span></span>|<span data-ttu-id="828a3-185">Int32</span><span class="sxs-lookup"><span data-stu-id="828a3-185">Int32</span></span>|<span data-ttu-id="828a3-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="828a3-186">The upload state.</span></span> <span data-ttu-id="828a3-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="828a3-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="828a3-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="828a3-188">publishingState</span></span>|[<span data-ttu-id="828a3-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="828a3-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="828a3-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="828a3-190">The publishing state for the app.</span></span> <span data-ttu-id="828a3-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="828a3-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="828a3-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="828a3-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="828a3-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="828a3-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="828a3-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="828a3-194">committedContentVersion</span></span>|<span data-ttu-id="828a3-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="828a3-195">String</span></span>|<span data-ttu-id="828a3-196">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="828a3-196">The internal committed content version.</span></span> <span data-ttu-id="828a3-197">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="828a3-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="828a3-198">fileName</span><span class="sxs-lookup"><span data-stu-id="828a3-198">fileName</span></span>|<span data-ttu-id="828a3-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="828a3-199">String</span></span>|<span data-ttu-id="828a3-200">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="828a3-200">The name of the main Lob application file.</span></span> <span data-ttu-id="828a3-201">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="828a3-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="828a3-202">size</span><span class="sxs-lookup"><span data-stu-id="828a3-202">size</span></span>|<span data-ttu-id="828a3-203">Int64</span><span class="sxs-lookup"><span data-stu-id="828a3-203">Int64</span></span>|<span data-ttu-id="828a3-204">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="828a3-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="828a3-205">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="828a3-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="828a3-206">commandLine</span><span class="sxs-lookup"><span data-stu-id="828a3-206">commandLine</span></span>|<span data-ttu-id="828a3-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="828a3-207">String</span></span>|<span data-ttu-id="828a3-208">A linha de comando.</span><span class="sxs-lookup"><span data-stu-id="828a3-208">The command line.</span></span>|
|<span data-ttu-id="828a3-209">productCode</span><span class="sxs-lookup"><span data-stu-id="828a3-209">productCode</span></span>|<span data-ttu-id="828a3-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="828a3-210">String</span></span>|<span data-ttu-id="828a3-211">O código do produto.</span><span class="sxs-lookup"><span data-stu-id="828a3-211">The product code.</span></span>|
|<span data-ttu-id="828a3-212">productVersion</span><span class="sxs-lookup"><span data-stu-id="828a3-212">productVersion</span></span>|<span data-ttu-id="828a3-213">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="828a3-213">String</span></span>|<span data-ttu-id="828a3-214">A versão de produto do aplicativo de linha de negócios (LoB) Windows Mobile MSI.</span><span class="sxs-lookup"><span data-stu-id="828a3-214">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="828a3-215">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="828a3-215">ignoreVersionDetection</span></span>|<span data-ttu-id="828a3-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="828a3-216">Boolean</span></span>|<span data-ttu-id="828a3-217">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="828a3-217">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="828a3-218">Defina como true para o aplicativos de linha de negócios (LoB) Windows Mobile MSI que usam um recurso de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="828a3-218">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="828a3-219">identityVersion</span><span class="sxs-lookup"><span data-stu-id="828a3-219">identityVersion</span></span>|<span data-ttu-id="828a3-220">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="828a3-220">String</span></span>|<span data-ttu-id="828a3-221">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="828a3-221">The identity version.</span></span>|
|<span data-ttu-id="828a3-222">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="828a3-222">useDeviceContext</span></span>|<span data-ttu-id="828a3-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="828a3-223">Boolean</span></span>|<span data-ttu-id="828a3-224">Indica se a instalação MSI um modo duplo no contexto do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="828a3-224">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="828a3-225">Se for true, aplicativo será instalado para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="828a3-225">If true, app will be installed for all users.</span></span> <span data-ttu-id="828a3-226">Se for false, o aplicativo será instalado por usuário.</span><span class="sxs-lookup"><span data-stu-id="828a3-226">If false, app will be installed per-user.</span></span> <span data-ttu-id="828a3-227">Se for null, serviço usará o contexto de instalação do pacote MSI padrão.</span><span class="sxs-lookup"><span data-stu-id="828a3-227">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="828a3-228">Em caso de modo duplo MSI, esse padrão serão por usuário.</span><span class="sxs-lookup"><span data-stu-id="828a3-228">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="828a3-229">Não podem ser definidas para aplicativos de modo não-duplo.</span><span class="sxs-lookup"><span data-stu-id="828a3-229">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="828a3-230">Não pode ser alterada após a criação inicial do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="828a3-230">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="828a3-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="828a3-231">Response</span></span>
<span data-ttu-id="828a3-232">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="828a3-232">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="828a3-233">Exemplo</span><span class="sxs-lookup"><span data-stu-id="828a3-233">Example</span></span>
### <a name="request"></a><span data-ttu-id="828a3-234">Solicitação</span><span class="sxs-lookup"><span data-stu-id="828a3-234">Request</span></span>
<span data-ttu-id="828a3-235">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="828a3-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 963

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
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

### <a name="response"></a><span data-ttu-id="828a3-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="828a3-236">Response</span></span>
<span data-ttu-id="828a3-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="828a3-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1126

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





