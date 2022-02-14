---
ms.localizationpriority: medium
ms.openlocfilehash: 04ba810183228e3834069d9bfa620fe3c71fdb12
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2022
ms.locfileid: "62805208"
---
<!-- markdownlint-disable MD002 MD025 MD041 -->

Crie tipos de resultados e verticais de pesquisa para personalizar os resultados da pesquisa no Microsoft SharePoint, Microsoft Office e Pesquisa da Microsoft no Bing, para facilitar que os usuários encontrem as informações que eles têm permissão para ver.

## <a name="create-a-vertical"></a>Criar uma vertical

Para criar e habilitar uma pesquisa vertical no nível da organização, entre no [](https://admin.microsoft.com/) centro de Administração Microsoft 365 usando a função de administrador global e faça o seguinte:

1. Vá para **Configurações** >  **Search &** **intelligenceCustomizations** > .
2. Vá para **Vertical** e clique no **botão Adicionar** .
3. Forneça os seguintes detalhes:
  * **Nomeia o vertical:** Partes do dispositivo.

   ![Captura de tela da seção "Nome da vertical"](images/connectors-images/build11.png)

  * **Fonte de** conteúdo: o conector criado com o aplicativo. (Inventário de Partes)

   ![Captura de tela da seção "Fonte de conteúdo"](images/connectors-images/build12.png)

  * **Adicione uma consulta**: deixe em branco.

   ![Captura de tela da seção "Adicionar uma consulta"](images/connectors-images/build13.png)

  * **Filtros**: deixe em branco.

   ![Captura de tela da seção "Filters"](images/connectors-images/build14.png)

## <a name="create-a-result-type"></a>Criar um tipo de resultado

Para criar um tipo de resultado:

1. Vá para **Configurações** >  **Search &** **intelligenceCustomizations** > .
2. Vá até a **guia tipo de** resultado e clique no **botão Adicionar** .
3. Forneça os seguintes detalhes:

  * **Nome**: Parte do Dispositivo

   ![Captura de tela da seção "Nomear o tipo de resultado"](images/connectors-images/build15.png)

  * **Fonte de** conteúdo: o conector criado no aplicativo.

   ![Captura de tela da seção "Selecionar uma fonte de conteúdo"](images/connectors-images/build16.png)

  * **Regras**: Nenhuma

   ![Captura de tela da seção "Definir regras"](images/connectors-images/build17.png)

  * Colar conteúdo de [result-type.json](https://github.com/microsoftgraph/msgraph-search-connector-sample/blob/master/result-type.json) na caixa de texto do designer de layout.

   ![Captura de tela da seção "Design layout"](images/connectors-images/build18.png)
