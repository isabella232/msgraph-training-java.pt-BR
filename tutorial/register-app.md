---
ms.openlocfilehash: 97763f135ab7529cfbcebf2eaf4d4d98d234fe10
ms.sourcegitcommit: 02054b307013cce781be2a3512ec1e54f1a322eb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2019
ms.locfileid: "35634728"
---
<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="bb3ca-101">Neste exercício, você criará um novo aplicativo do Azure AD usando o centro de administração do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bb3ca-101">In this exercise you will create a new Azure AD application using the Azure Active Directory admin center.</span></span>

1. <span data-ttu-id="bb3ca-102">Abra um navegador, navegue até o [centro de administração do Azure Active Directory](https://aad.portal.azure.com) e faça logon usando uma **conta pessoal** (também conhecida como conta da Microsoft) ou **Conta Corporativa ou de Estudante**.</span><span class="sxs-lookup"><span data-stu-id="bb3ca-102">Open a browser and navigate to the [Azure Active Directory admin center](https://aad.portal.azure.com) and login using a **personal account** (aka: Microsoft Account) or **Work or School Account**.</span></span>

1. <span data-ttu-id="bb3ca-103">Selecione **Azure Active Directory** na navegação à esquerda e, em seguida, selecione **registros de aplicativo** em **gerenciar**.</span><span class="sxs-lookup"><span data-stu-id="bb3ca-103">Select **Azure Active Directory** in the left-hand navigation, then select **App registrations** under **Manage**.</span></span>

    ![<span data-ttu-id="bb3ca-104">Uma captura de tela dos registros de aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb3ca-104">A screenshot of the App registrations</span></span> ](./images/aad-portal-app-registrations.png)

1. <span data-ttu-id="bb3ca-105">Selecione **Novo registro**.</span><span class="sxs-lookup"><span data-stu-id="bb3ca-105">Select **New registration**.</span></span> <span data-ttu-id="bb3ca-106">Na página **Registrar um aplicativo**, defina os valores da seguinte forma.</span><span class="sxs-lookup"><span data-stu-id="bb3ca-106">On the **Register an application** page, set the values as follows.</span></span>

    - <span data-ttu-id="bb3ca-107">Defina **Nome** para `Java Graph Tutorial`.</span><span class="sxs-lookup"><span data-stu-id="bb3ca-107">Set **Name** to `Java Graph Tutorial`.</span></span>
    - <span data-ttu-id="bb3ca-108">Defina os **tipos de conta com suporte** para **contas em qualquer diretório organizacional**.</span><span class="sxs-lookup"><span data-stu-id="bb3ca-108">Set **Supported account types** to **Accounts in any organizational directory**.</span></span>
    - <span data-ttu-id="bb3ca-109">Deixe o **URI de Redirecionamento** vazio.</span><span class="sxs-lookup"><span data-stu-id="bb3ca-109">Leave **Redirect URI** empty.</span></span>

    ![Uma captura de tela da página registrar um aplicativo](./images/aad-register-an-app.png)

1. <span data-ttu-id="bb3ca-111">Escolha **Registrar**.</span><span class="sxs-lookup"><span data-stu-id="bb3ca-111">Choose **Register**.</span></span> <span data-ttu-id="bb3ca-112">Na página **tutorial do Java Graph** , copie o valor da **ID do aplicativo (cliente)** e salve-o, você precisará dele na próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="bb3ca-112">On the **Java Graph Tutorial** page, copy the value of the **Application (client) ID** and save it, you will need it in the next step.</span></span>

    ![Uma captura de tela da ID do aplicativo do novo registro de aplicativo](./images/aad-application-id.png)

1. <span data-ttu-id="bb3ca-114">Selecione o link **Adicionar um URI** de redirecionamento.</span><span class="sxs-lookup"><span data-stu-id="bb3ca-114">Select the **Add a Redirect URI** link.</span></span> <span data-ttu-id="bb3ca-115">Na página **redirecionar URIs** , localize a seção redirecionar **URIs sugeridos para clientes públicos (móvel, área de trabalho)** .</span><span class="sxs-lookup"><span data-stu-id="bb3ca-115">On the **Redirect URIs** page, locate the **Suggested Redirect URIs for public clients (mobile, desktop)** section.</span></span> <span data-ttu-id="bb3ca-116">Selecione o `https://login.microsoftonline.com/common/oauth2/nativeclient` URI.</span><span class="sxs-lookup"><span data-stu-id="bb3ca-116">Select the `https://login.microsoftonline.com/common/oauth2/nativeclient` URI.</span></span>

    ![Captura de tela da página URIs de redirecionamento](./images/aad-redirect-uris.png)

1. <span data-ttu-id="bb3ca-118">Localize a seção **tipo de cliente padrão** e altere o **aplicativo tratar como um cliente público** alternar para **Sim**e, em seguida, escolha **salvar**.</span><span class="sxs-lookup"><span data-stu-id="bb3ca-118">Locate the **Default client type** section and change the **Treat application as a public client** toggle to **Yes**, then choose **Save**.</span></span>

    ![Uma captura de tela da seção tipo de cliente padrão](./images/aad-default-client-type.png)