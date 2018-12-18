---
title: Criar windowsMobileMSI
description: Cria um novo objeto windowsMobileMSI.
author: tfitzmac
ms.openlocfilehash: 6c3ba27b3b6009bf25fc98f2ee5151991fedca19
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353106"
---
# <a name="create-windowsmobilemsi"></a><span data-ttu-id="3164b-103">Criar windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="3164b-103">Create windowsMobileMSI</span></span>

> <span data-ttu-id="3164b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3164b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3164b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3164b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3164b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3164b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3164b-107">Cria um novo objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="3164b-107">Create a new [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3164b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3164b-108">Prerequisites</span></span>
<span data-ttu-id="3164b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3164b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3164b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3164b-111">Permission type</span></span>|<span data-ttu-id="3164b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3164b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3164b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3164b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3164b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3164b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3164b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3164b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3164b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3164b-116">Not supported.</span></span>|
|<span data-ttu-id="3164b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3164b-117">Application</span></span>|<span data-ttu-id="3164b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3164b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3164b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3164b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3164b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3164b-120">Request headers</span></span>
|<span data-ttu-id="3164b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3164b-121">Header</span></span>|<span data-ttu-id="3164b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3164b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3164b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3164b-123">Authorization</span></span>|<span data-ttu-id="3164b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3164b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3164b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3164b-125">Accept</span></span>|<span data-ttu-id="3164b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3164b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3164b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3164b-127">Request body</span></span>
<span data-ttu-id="3164b-128">No corpo da solicitação, forneça uma representação JSON para o objeto windowsMobileMSI.</span><span class="sxs-lookup"><span data-stu-id="3164b-128">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="3164b-129">A tabela a seguir mostra as propriedades obrigatórias ao criar windowsMobileMSI.</span><span class="sxs-lookup"><span data-stu-id="3164b-129">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="3164b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3164b-130">Property</span></span>|<span data-ttu-id="3164b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3164b-131">Type</span></span>|<span data-ttu-id="3164b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3164b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3164b-133">id</span><span class="sxs-lookup"><span data-stu-id="3164b-133">id</span></span>|<span data-ttu-id="3164b-134">String</span><span class="sxs-lookup"><span data-stu-id="3164b-134">String</span></span>|<span data-ttu-id="3164b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3164b-135">Key of the entity.</span></span> <span data-ttu-id="3164b-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3164b-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3164b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3164b-137">displayName</span></span>|<span data-ttu-id="3164b-138">String</span><span class="sxs-lookup"><span data-stu-id="3164b-138">String</span></span>|<span data-ttu-id="3164b-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="3164b-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3164b-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3164b-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3164b-141">description</span><span class="sxs-lookup"><span data-stu-id="3164b-141">description</span></span>|<span data-ttu-id="3164b-142">String</span><span class="sxs-lookup"><span data-stu-id="3164b-142">String</span></span>|<span data-ttu-id="3164b-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3164b-143">The description of the app.</span></span> <span data-ttu-id="3164b-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3164b-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3164b-145">publisher</span><span class="sxs-lookup"><span data-stu-id="3164b-145">publisher</span></span>|<span data-ttu-id="3164b-146">String</span><span class="sxs-lookup"><span data-stu-id="3164b-146">String</span></span>|<span data-ttu-id="3164b-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3164b-147">The publisher of the app.</span></span> <span data-ttu-id="3164b-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3164b-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3164b-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3164b-149">largeIcon</span></span>|[<span data-ttu-id="3164b-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3164b-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3164b-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="3164b-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3164b-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3164b-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3164b-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3164b-153">createdDateTime</span></span>|<span data-ttu-id="3164b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3164b-154">DateTimeOffset</span></span>|<span data-ttu-id="3164b-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3164b-155">The date and time the app was created.</span></span> <span data-ttu-id="3164b-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3164b-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3164b-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3164b-157">lastModifiedDateTime</span></span>|<span data-ttu-id="3164b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3164b-158">DateTimeOffset</span></span>|<span data-ttu-id="3164b-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3164b-159">The date and time the app was last modified.</span></span> <span data-ttu-id="3164b-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3164b-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3164b-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3164b-161">isFeatured</span></span>|<span data-ttu-id="3164b-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="3164b-162">Boolean</span></span>|<span data-ttu-id="3164b-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3164b-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3164b-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3164b-164">privacyInformationUrl</span></span>|<span data-ttu-id="3164b-165">String</span><span class="sxs-lookup"><span data-stu-id="3164b-165">String</span></span>|<span data-ttu-id="3164b-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="3164b-166">The privacy statement Url.</span></span> <span data-ttu-id="3164b-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3164b-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3164b-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3164b-168">informationUrl</span></span>|<span data-ttu-id="3164b-169">String</span><span class="sxs-lookup"><span data-stu-id="3164b-169">String</span></span>|<span data-ttu-id="3164b-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="3164b-170">The more information Url.</span></span> <span data-ttu-id="3164b-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3164b-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3164b-172">owner</span><span class="sxs-lookup"><span data-stu-id="3164b-172">owner</span></span>|<span data-ttu-id="3164b-173">String</span><span class="sxs-lookup"><span data-stu-id="3164b-173">String</span></span>|<span data-ttu-id="3164b-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="3164b-174">The owner of the app.</span></span> <span data-ttu-id="3164b-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3164b-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3164b-176">developer</span><span class="sxs-lookup"><span data-stu-id="3164b-176">developer</span></span>|<span data-ttu-id="3164b-177">String</span><span class="sxs-lookup"><span data-stu-id="3164b-177">String</span></span>|<span data-ttu-id="3164b-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3164b-178">The developer of the app.</span></span> <span data-ttu-id="3164b-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3164b-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3164b-180">Observações</span><span class="sxs-lookup"><span data-stu-id="3164b-180">notes</span></span>|<span data-ttu-id="3164b-181">String</span><span class="sxs-lookup"><span data-stu-id="3164b-181">String</span></span>|<span data-ttu-id="3164b-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3164b-182">Notes for the app.</span></span> <span data-ttu-id="3164b-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3164b-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3164b-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="3164b-184">uploadState</span></span>|<span data-ttu-id="3164b-185">Int32</span><span class="sxs-lookup"><span data-stu-id="3164b-185">Int32</span></span>|<span data-ttu-id="3164b-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="3164b-186">The upload state.</span></span> <span data-ttu-id="3164b-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3164b-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3164b-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="3164b-188">publishingState</span></span>|[<span data-ttu-id="3164b-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3164b-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3164b-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3164b-190">The publishing state for the app.</span></span> <span data-ttu-id="3164b-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="3164b-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3164b-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3164b-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="3164b-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="3164b-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3164b-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="3164b-194">committedContentVersion</span></span>|<span data-ttu-id="3164b-195">String</span><span class="sxs-lookup"><span data-stu-id="3164b-195">String</span></span>|<span data-ttu-id="3164b-196">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="3164b-196">The internal committed content version.</span></span> <span data-ttu-id="3164b-197">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="3164b-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3164b-198">fileName</span><span class="sxs-lookup"><span data-stu-id="3164b-198">fileName</span></span>|<span data-ttu-id="3164b-199">String</span><span class="sxs-lookup"><span data-stu-id="3164b-199">String</span></span>|<span data-ttu-id="3164b-200">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="3164b-200">The name of the main Lob application file.</span></span> <span data-ttu-id="3164b-201">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="3164b-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3164b-202">size</span><span class="sxs-lookup"><span data-stu-id="3164b-202">size</span></span>|<span data-ttu-id="3164b-203">Int64</span><span class="sxs-lookup"><span data-stu-id="3164b-203">Int64</span></span>|<span data-ttu-id="3164b-204">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="3164b-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="3164b-205">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="3164b-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3164b-206">commandLine</span><span class="sxs-lookup"><span data-stu-id="3164b-206">commandLine</span></span>|<span data-ttu-id="3164b-207">String</span><span class="sxs-lookup"><span data-stu-id="3164b-207">String</span></span>|<span data-ttu-id="3164b-208">A linha de comando.</span><span class="sxs-lookup"><span data-stu-id="3164b-208">The command line.</span></span>|
|<span data-ttu-id="3164b-209">productCode</span><span class="sxs-lookup"><span data-stu-id="3164b-209">productCode</span></span>|<span data-ttu-id="3164b-210">String</span><span class="sxs-lookup"><span data-stu-id="3164b-210">String</span></span>|<span data-ttu-id="3164b-211">O código do produto.</span><span class="sxs-lookup"><span data-stu-id="3164b-211">The product code.</span></span>|
|<span data-ttu-id="3164b-212">productVersion</span><span class="sxs-lookup"><span data-stu-id="3164b-212">productVersion</span></span>|<span data-ttu-id="3164b-213">String</span><span class="sxs-lookup"><span data-stu-id="3164b-213">String</span></span>|<span data-ttu-id="3164b-214">A versão de produto do aplicativo de linha de negócios (LoB) Windows Mobile MSI.</span><span class="sxs-lookup"><span data-stu-id="3164b-214">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="3164b-215">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="3164b-215">ignoreVersionDetection</span></span>|<span data-ttu-id="3164b-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="3164b-216">Boolean</span></span>|<span data-ttu-id="3164b-217">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3164b-217">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="3164b-218">Defina como true para o aplicativos de linha de negócios (LoB) Windows Mobile MSI que usam um recurso de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="3164b-218">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="3164b-219">identityVersion</span><span class="sxs-lookup"><span data-stu-id="3164b-219">identityVersion</span></span>|<span data-ttu-id="3164b-220">String</span><span class="sxs-lookup"><span data-stu-id="3164b-220">String</span></span>|<span data-ttu-id="3164b-221">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="3164b-221">The identity version.</span></span>|
|<span data-ttu-id="3164b-222">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="3164b-222">useDeviceContext</span></span>|<span data-ttu-id="3164b-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="3164b-223">Boolean</span></span>|<span data-ttu-id="3164b-224">Indica se a instalação MSI um modo duplo no contexto do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3164b-224">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="3164b-225">Se for true, aplicativo será instalado para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="3164b-225">If true, app will be installed for all users.</span></span> <span data-ttu-id="3164b-226">Se for false, o aplicativo será instalado por usuário.</span><span class="sxs-lookup"><span data-stu-id="3164b-226">If false, app will be installed per-user.</span></span> <span data-ttu-id="3164b-227">Se for null, serviço usará o contexto de instalação do pacote MSI padrão.</span><span class="sxs-lookup"><span data-stu-id="3164b-227">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="3164b-228">Em caso de modo duplo MSI, esse padrão serão por usuário.</span><span class="sxs-lookup"><span data-stu-id="3164b-228">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="3164b-229">Não podem ser definidas para aplicativos de modo não-duplo.</span><span class="sxs-lookup"><span data-stu-id="3164b-229">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="3164b-230">Não pode ser alterada após a criação inicial do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3164b-230">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="3164b-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="3164b-231">Response</span></span>
<span data-ttu-id="3164b-232">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3164b-232">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3164b-233">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3164b-233">Example</span></span>
### <a name="request"></a><span data-ttu-id="3164b-234">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3164b-234">Request</span></span>
<span data-ttu-id="3164b-235">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3164b-235">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1018

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

### <a name="response"></a><span data-ttu-id="3164b-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="3164b-236">Response</span></span>
<span data-ttu-id="3164b-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3164b-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





